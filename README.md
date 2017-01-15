# sass
基于sass的技术，模块化开发css
## install
Sass官网：http://sass-lang.com/install

* 环境依赖ruby
* linux & macOs install
```shell
sudo gem install sass
```

## 项目结构
* project    
  * sass   
    * component    
      * button.scss    
    * helpers    
      * mixin.scss   
    * themes   
      * theme.scss   
    * main.scss    
  * index.html   

## code
部分 scss 代码展示
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
