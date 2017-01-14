# sass
基于sass 模块化开发css demo
## install
http://sass-lang.com/install

## code
main.scss
```scss
@import "layout/layout";
@import "component/button";
@import "themes/theme";
```
layout.scss
```scss
@import "../helpers/mixin";

.row{
  padding: 5px;
  width:100%;
}
...
.col-md-11{
  @extend .col-md;
  @include col_md(11);
}
```
## start
npm run sass
