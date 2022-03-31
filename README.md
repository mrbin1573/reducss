# reducss（reduce css）

> 将常用的 css 进行全局封装，让你写更少的 css，更专注于处理业务逻辑

## 封装了如下模块

- 尺寸相关
  - margin
  - padding
  - border-radius
  - font-size
- flex 布局

## 使用

- 默认单位为 px
- `rem`：在名称和值中间添加`rem`即可（`mt-rem-10`表示`margin-top: 10rem`）

### margin

```scss
  .mg-{size} => margin: {size}px;
  .mt-{size} => margin: {size}px 0 0 0;
  .mr-{size} => margin: 0 {size}px 0 0;
  .mb-{size} => margin: 0 0 {size}px 0;
  .ml-{size} => margin: 0 0 0 {size}px;
```

### padding

```scss
.pd-${size} => padding: ${size}px;
.pt-${size} => padding: ${size}px 0 0 0;
.pr-${size} => padding: 0 ${size}px 0 0;
.pb-${size} => padding: 0 0 ${size}px 0;
.pl-${size} => padding: 0 0 0 ${size}px;
```

### font-size

```scss
.font-${size} => font-size: ${size}px;
```

### border-radius

会自动加上`overflow: hidden;`

```css
.radius-${size} => border-radius: ${size}px
```
