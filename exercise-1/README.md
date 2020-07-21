## 需求说明

### 完成下列选择题，请将答案写到每题后面括号里

1.在下列选择器中，哪一个代表 section class 里面的所有 title class? (A)

A <lable>.section .title {}</lable>  
B <lable>.section.title {}</lable>  
C <lable>.section, .title {}</lable>  
D <lable>.section > .title {}</lable>  

2.在下列选择器中，哪一个代表 section class 内部紧邻的 title class? (D)

A <lable>.section .title {}</lable>  
B <lable>.section.title {}</lable>   
C <lable>.section, .title {}</lable>   
D <lable>.section > .title {}</lable>  

3.在下列选择器中，哪一个代表同一个元素同时拥有 section 和 title 两个class? ( B)

A <lable>.section .title {}</lable>  
B <lable>.section.title {}</lable>   
C <lable>.section, .title {}</lable>   
D <lable>.section > .title {}</lable>   

4.在下列选择器中，哪一个代表 section 和 title 两个class 设置相同样式? ( C)

A <lable>.section .title {}</lable>  
B <lable>.section.title {}</lable>   
C <lable>.section, .title {}</lable>   
D <lable>.section > .title {}</lable>   

------

后代选择器：选择作为某元素后代的元素。 在后代选择器中，规则左边的选择器一端包括两个或多个用空格分隔的选择器，即A表示section class 里面的所有 title class，B的选择器未用空格隔开，不是后代选择器，代表的是一个class=“section title”的元素；

选择器分组：为了使多个选择器拥有相同的样式，可以用逗号将两个选择器进行隔开，进行分组，即C表示section和title同时满足相同的样式；

子元素选择器：比后代选择器范围要小，通过使用大于号（两边空白符可选），只选择某个元素的子元素，即D表示title class 作为section class的子元素，满足一定的样式。

------

5.在下列CSS选择器中，优先级从高到低是：(2)

```
<div class="section">
    <h1 id="title" class="title">title</div>
</div>

A)  .section .title { color:red; }
B)  #title { color:green; }
C)  .title { color:yellow !important; }
D)  .section > h1 { color:blue; }
```
1)  <lable> B > C > D > A </lable>   
2)  <lable> C > B > A > D </lable>    
3)  <lable> D > B > A > C</lable>  
4)  <lable> 以上都不对 </lable>  

  

## 本练习知识点

- CSS can change the look of HTML elements. In order to do this, CSS must select HTML elements, then apply styles to them.
- CSS can select HTML elements by tag, class, or ID.
- Multiple CSS classes can be applied to one HTML element.
- Classes can be reusable, while IDs can only be used once.
- IDs are more specific than classes, and classes are more specific than tags. That means IDs will override any styles from a class, and classes will override any styles from a tag selector.
- Multiple selectors can be chained together to select an element. This raises the specificity, but can be necessary.
- Nested elements can be selected by separating selectors with a space.
- The `!important` flag will override any style, however it should almost never be used, as it is extremely difficult to override.
- Multiple unrelated selectors can receive the same styles by separating the selector names with commas.

