# React-Document

## ทบทวน

### Pure Function

มีคุณสมบัติดังต่อไปนี้

        function add(x, y) {
          return x + y;
        }


### Higher-order Function

### Arrow Function

Arrow Function ช่วยให้เราสามารถเขียนไวยากรณ์ฟังก์ชั่นที่สั้นลงและยังมีความสามารถเข้าถึง this จาก scope ที่ครอบมันอยู่ ซึ่งมีมาให้ใน ES6

-   Before

        hello = function() {
          return "Hello World!";
        }
    
-   Arrow Function

        hello = () => {
          return "Hello World!";
        }
        
### Map Function

### Filter Function


## Lifecycle method

![g6LQe](https://user-images.githubusercontent.com/15135199/73858354-d675d080-486a-11ea-9f59-aee84189e526.png)

## Stateless Component vs Class Component

![image](https://user-images.githubusercontent.com/15135199/73670193-5ff69880-46db-11ea-9dcb-2717320fa3fa.png)


### โครงสร้างไฟล์ที่สำคัญของ React

- public/index.html : คือไฟล์ html หลัก web

- src/index.js : เป็นไฟล์หลักของ React

- src/App.js : ไฟล์สำหรับ Component ที่ชื่อว่า App

### dependencies

- react-viewer

## Reference

- https://ihatetomatoes.net/react-tutorial-for-beginners/
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment
- https://60devs.com/pure-component-in-react.html
- https://www.babelcoder.com/blog/posts/introduction-to-es2015
- https://reactpatterns.com/
- https://github.com/chantastic/react-patterns
- https://github.com/chantastic/reactpatterns#stateless-function
- https://microbenz.in.th/%E0%B8%97%E0%B8%B3%E0%B8%84%E0%B8%A7%E0%B8%B2%E0%B8%A1%E0%B8%A3%E0%B8%B9%E0%B9%89%E0%B8%88%E0%B8%B1%E0%B8%81%E0%B8%81%E0%B8%B1%E0%B8%9A-redux-%E0%B9%81%E0%B8%9A%E0%B8%9A%E0%B8%89%E0%B8%9A%E0%B8%B1%E0%B8%9A%E0%B8%A2%E0%B9%88%E0%B8%AD%E0%B8%A2%E0%B9%81%E0%B8%A5%E0%B9%89%E0%B8%A7%E0%B8%A2%E0%B9%88%E0%B8%AD%E0%B8%A2%E0%B8%AD%E0%B8%B5%E0%B8%81-b464808aca12
- https://reactjs.org/docs/fragments.html
- https://github.com/JedWatson/classnames
- https://upmostly.com/tutorials/react-onclick-event-handling-with-examples
- https://stackoverflow.com/questions/43087007/react-link-vs-a-tag-and-arrow-function
- https://medium.com/@learnreact/container-components-c0e67432e005
- https://web.dev/code-splitting-suspense/
- https://www.youtube.com/watch?v=QFaFIcGhPoM&list=PLC3y8-rFHvwgg3vaYJgHGnModB54rxOk3&index=1
- https://medium.com/@konstankino/2019-reactjs-best-practices-design-patterns-516e1c3ca06a
- https://stackoverflow.com/questions/49162311/react-difference-between-route-exact-path-and-route-path
