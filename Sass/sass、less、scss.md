# sass

## 一、变量

老版本使用!，与css有冲突，改为==$==

## 二、嵌套规则

1. 父选择器的标识符&；

   ```scss
   //伪类
   article a {
     color: blue;
     &:hover { color: red }
   }
   /*编译后*/
   article a { color: blue }
   article a:hover { color: red }
   
   //在父选择器之前添加选择器
   #content aside {
     color: red;
     body.ie & { color: green }
   }
   /*编译后*/
   #content aside {color: red};
   body.ie #content aside { color: green }
   ```

2. 群组选择器的嵌套;

   ```scss
   
   ```

   





# sass、less、scss区别

1. sass与scss区别是，sass是2.0及以前的，使用==缩进语法==

2. sass定义变量使用$，less使用@

3. sass支持如下，less不行

   ```
   $link-color: blue;
   a {
     color: $link_color;
   }
   ```

4. 