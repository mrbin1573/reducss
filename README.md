# reducss（reduce css）

> 一个对常用的 css 进行封装的简单库，采用 scss 语言，让你写更少的 css，更专注于处理业务逻辑

# 安装使用

## 安装

```cmd
npm install reducss
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
  默认 2~20 偶数值
- padding: `pd-x` `pt-x` `pr-r` `pb-x` `pl-x`
  默认 2~20 偶数值
- radius: `r-x`
  默认 2~20 偶数值
- fontSize: `fs-x`
  默认 8~30 偶数值
- fontWight: `fw-x`
  默认 100~1000 以及`thin` `lighter` `light` `normal` `medium` `bold` `bolder`
- position

# 优缺点

## 优点

- 😊 高度自定义；`variable.scss`中可修改自己需要的尺寸，单位；以适应不同的场景
- 😊 写更少的`css`；解放双手，更专注业务逻辑
- 😊 代码量更少；直接使用全局`css`，减少大量重复属性

## 缺点

- 😔 会有用不上的`css`；和减少的代码量相比微不足道，还可通过`variable.scss`减少无用代码
- 😔 需要花少量时间熟记 `class` 属性，不过都是首字母缩写很好记忆
