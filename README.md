# reducss（reduce css）

> 一个对常用的 css 进行封装的简单库，采用 scss 语言，让你写更少的 css，更专注于处理业务逻辑

# 安装使用

## 安装

```cmd
npm install reducss
```

main.js 中引入

```js
import "reducss"
```

## 使用

### 示例

```hmtl
<div class="mt-10 pd-10 radius-20 fs-20 fw-bold"></div>
```

### 可用项

- flex: `flex-xx`

  - flex-row: flex-direction: row;
  - flex-column: flex-direction: column;
  - flex-mid: align-items: center;
  - flex-center: justify-content: center;
  - flex-between: justify-content: space-between;
  - flex-around: justify-content: space-around;
  - flex-grow-1: flex-grow: 1;
  - flex-grow-0: flex-grow: 0;
  - flex-shrink-1: flex-shrink: 1;
  - flex-shrink-0: flex-shrink: 0;

- margin: `mg-x` `mt-x` `mr-x` `mb-x` `ml-x`
- padding: `pd-x` `pt-x` `pr-r` `pb-x` `pl-x`
- radius: `radius-x`
  会自动添加`overflow: hidden`
  额外的值（p 是 percent 的缩写）
  - radius-50p：`border-radius: 50%`
  - radius-10p：`border-radius: 100%`
- fontSize: `fs-x`
- fontWight: `fw-x`
- position: 直接使用`static` `relative` `absolute` `sticky` `fixed` `inline` `inline-block`

### 自定义变量

在项目全局定义以下 `scss` 变量即可覆盖封装的值（内部会按如下变量循环，需要列出所有你使用的值），修改值可能需要重启才能生效
以下为封装的所有原始可用值

```scss
$suffix: "px"; // 尺寸的单位,可替换为em rem rpx等任意单位

$marginSize: 2, 4, 6, 8, 10, 12, 14, 16, 18, 20;

$paddingSize: 2, 4, 6, 8, 10, 12, 14, 16, 18, 20;

$radiusSize: 2, 4, 6, 8, 10, 12, 14, 16, 18, 20;

$fontSize: 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30;

$fontWeight: 100, 200, 300, 400, 500, 600, 700, 800, 900, 1000, thin, lighter, light, normal, medium, bold, bolder;
```

# 优缺点

## 优点

- 😊 高度自定义；`variable.scss`中可修改自己需要的尺寸，单位；以适应不同的场景
- 😊 写更少的`css`；解放双手，更专注业务逻辑
- 😊 代码量更少；直接使用全局`css`，减少大量重复属性

## 缺点

- 😔 会有用不上的`css`；和减少的代码量相比微不足道，还可通过`variable.scss`减少无用代码
- 😔 需要花少量时间熟记 `class` 属性，不过都是首字母缩写很好记忆
