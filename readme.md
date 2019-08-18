## 前端一些技巧

### 几个技巧
   1. Google 关键词
      1. CSS Tricks
      2. 阮一峰
      3. 张鑫旭
      4. Codrops 炫酷效果
      5. CSS揭秘
      6. mdn
      7. wall haven 背景图
      8. iconfont
   2. 解决浮动横排的 下排的元素会环绕的bug
```
在父标签上加上这个样式
.clearfix::after {
    content: "";
    display: block;
    clear: both;
}
```
   3. 伪类添加边框抖动bug
      1. 先加上边框，吧边框设置成透明
      2. 边框透明：border:1px solid transparent; 
   4. 背景图自适应
      1. background-size:cover;
   5. 内元素超出外元素bug
      1. 在内元素加 display:block
   6. div高度是由内部文档流的高度总和决定的
      1. 文档流：文档内元素流动的方向
      2. 内联元素从左往右流，直到换行
      3. 块级元素是从上往下流
   7. 脱离文档流
      1. position: fixed 相对于屏幕固定
      2. 脱离文档流后div的宽度会向左缩进，这时可以用width:100%解决，但是这是一个隐藏的bug
   8. div宽度写死如果给这个div的padding和div本身的宽度大于父宽度会超出父宽度，解决方法在div和div父标签之间加一个div让她们隔两代
   9. 居中
      1. 如果一个div宽度写死想要居中：
         1. margin-left:auto;
         2. margin-right:auto;

### 几个效果

1. sticky nabar  黏糊导航
2. auto highLight navbar 导航自动响应
3. auto scroll smoothly 自动跳转滚动
4. menu 下拉菜单
5. auto hide aside 自动隐藏侧边栏
6. loading animation 加载动画
7. animate when scroll 滚动动画