# reducss（reduce css）

> 一个对常用的 css 进行封装的简单库，采用 scss 语言，让你写更少的 css，更专注于处理业务逻辑

```hmtl
<div class="mt-10 pd-10 radius-20 fs-20 fw-bold"></div>
```

# 优缺点

## 优点

- 😊 高度自定义；`variable.scss`中可修改自己需要的尺寸，单位；以适应不同的场景
- 😊 写更少的`css`；解放双手，更专注业务逻辑
- 😊 代码量更少；直接使用全局`css`，减少大量重复属性

## 缺点

- 😔 会有用不上的`css`；和减少的代码量相比微不足道
- 😔 对`vue scoped`不友好；使用`scoped`生成`data-xxx`的 css

# 可使用属性

- 尺寸相关
  - margin
  - padding
  - border-radius
  - font-size
- flex 布局
- position
