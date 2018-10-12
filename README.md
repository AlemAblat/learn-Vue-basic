## 					Vue 初学教程



### 课程介绍

- 本课程是记录我个人从0开始学习经验
- 可以通过本课程通俗易懂的掌握Vue基本开发
- 用实战实例让学员们感受Vue的魅力

### 要学习Vue要有一下知识点

- HTML基础
- CSS基础
- JaveScript基础
- 基本命令行基础（cd, ls, mv, vi ...）

### 什么是Vue

- Vue.js 是前端的**主流框架之一**，和Angular.js、React.js 一起，并成为前端三大主流框架！
- Vue.js 是一套构建用户界面的框架，**只关注视图层**，它不仅易于上手，还便于与第三方库或既有项目整合。（Vue有配套的第三方类库，可以整合起来做大型项目的开发）并且开发人员不要再操作DOM了，可以释放双手精简的框架
- 前端的主要工作？主要负责MVC中的V这一层；主要工作就是和界面打交道，来制作前端页面效果；



### 1.引入VueJs框架

---

- 远程引入方式

```html
<!-- development version, includes helpful console warnings -->
<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
```

or:

```html
<!-- production version, optimized for size and speed -->
<script src="https://cdn.jsdelivr.net/npm/vue"></script>
```

- #### 本地引入方式
```html
<!-- Local include VueJs Framework -->
<script src="./assets/js/vue.js"></script>
```
```diff
- !! 引入框架在我们HTML文档的head标签里面，也就是通常引入JS和央视文件CSS的方式一样 !!
```

### 2. 我们来实例来Hello World !

- 首先创建html文件

     

  ```html
  <!DOCTYPE html>
  <html lang="en">
  
  <head>
      <meta charset="UTF-8">
      <title>Vue Js</title>
          <!-- 引入开发版本VueJs框架 -->
      <!-- development version, includes helpful console warnings -->
      <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
  </head>
  
  <body>
          <!-- 创建div并里面引入Vue的变量msg -->
  
      <div id="app">
      <!-- 引入变量msg -->
  	{{ msg }}
      </div>
         
   <!--创建script标签 -->  
    <script type="text/javascript">
    	// 实例化框架
    	var vue = new Vue({
    		//元素属性，用元素的ID来获取
    		el: "#app",
    		//数据属性，数据属性是一个对象
    		data:{
    			// 创建变量msg
    			msg: "Hello World !"
    		}
      })
    </script>
  </body>
  
  </html>
  ```


