# React-Document

## React Lifecycle methods คืออะไร

React Lifecycle methods คือ ลำดับของเหตุการณ์ที่เกิดขึ้นตั้งแต่จุดเริ่มต้นของ React component จนถึงตอนสิ้นสุด ทุก Component ใน React ควรมีวงจรชีวิตของเหตุการณ์ต่อไปนี้

   - ##### Mounting คือการเกิดขึ้นของ Component

   - ##### Updating คือการเติบโตหรือเปลี่ยนแปลงของ Component
   
   - ##### Unmounting คือจุดสิ้นสุดของ Component

#### 1. Render () : method

      Render method คือทำหน้าที่จัดการการเรนเดอร์ Component ของเราในขณะเข้าถึงหรือเปลี่ยนแปลง state หรือ props เราจะไม่สามารถเรียกใช้ 
      setState method ได้ใน render method 

#### 2. Constructor () : method

      Constructor method คือ method ที่ถูกเรียกก่อน method อื่นๆ เมื่อใช้ Constructor ควรเรียกใช้ super(props) ก่อน statement อื่นๆทั้งหมด
      มิฉะนั้น this.props จะเป็น undefined ซึ่งอาจนำไปสู่ข้อผิดพลาดที่สำคัญในแอปพลิเคชัน การใช้ Constructor ส่วนใหญ่เกิดจากเหตุผลดังต่อไปนี้

   - Initializing the state
   
   - binding our component

#### 3. ComponentDidMount() : method

#### 4. ComponentWillMount() : method

      จะถูกดำเนินการก่อนการ Render

#### 5. ComponentWillReceiveProps() : method

#### 6. ShouldComponentUpdate() : method

#### 7. ComponentWillUpdate () : method

#### กรณีโหลดหน้าครั้งแรก
<p align="center">
  <img src="https://user-images.githubusercontent.com/15135199/91645429-2b7b6d00-ea6f-11ea-968d-1c49458c4093.jpg"  height=300px">
</p>

#### กรณี Props มีการเปลี่ยนแปลง
<p align="center">
  <img src="https://user-images.githubusercontent.com/15135199/91645626-d93b4b80-ea70-11ea-8ee2-d106e94e113d.png" height=400px">
</p>

#### กรณี State มีการเปลี่ยนแปลง
<p align="center">
  <img src="https://user-images.githubusercontent.com/15135199/91645736-e9075f80-ea71-11ea-8c50-6ac0cc2bdac6.png" height=300px">
</p>


### Statefull Component vs Stateless Component

- #### Statefull Component

  Statefull Component คือ Component ที่มี state จัดเก็บข้อมูลเกี่ยวกับการเปลี่ยนแปลง state ของ Component ในหน่วยความจำ

- #### Stateless Component

### Container Components vs Presentational Components

- #### Container Component

- #### Presentational Component

### โครงสร้างไฟล์ที่สำคัญของ React

- public/index.html : คือไฟล์ html หลัก web

- src/index.js : เป็นไฟล์หลักของ React

- src/App.js : ไฟล์สำหรับ Component ที่ชื่อว่า App

### วิธีเปลี่ยนเส้นทางจากหน้าหนึ่งไปอีกหน้า

- using Redirect component

        import React from 'react';
        import {Redirect} from 'react-router-dom';

        class Login extends React.Component {

          onSubmit = () => {
             if(userFound){
                 return  <Redirect  to="/posts/" />
             }
          }

          render() {
            return (
              <form>
                <input placeholder="email" type="email" />
                <input placeholder="password" type="password" />
                <button onClick={this.onSubmit}>Login</button>
              </form>
            )
          }
        }

        export default Login;
      
- using history object
    
        import React from 'react';
        class Login extends React.Component {

          onSubmit = () => {
             if(userFound){
                 this.props.history.push('/posts/');
             }
          }

          render() {
            return (
              <form>
                <input placeholder="email" type="email" />
                <input placeholder="password" type="password" />
                <button onClick={this.onSubmit}>Login</button>
              </form>
            )
          }
        }

        export default Login;

### Local Storage

-  overview of localStorage methods.

| Method      | Description |
| ------------- | ------------- |
| setItem(key, value)  | Add key and value to local storage  |
| getItem(key)  | Retrieve a value by the key  |
| removeItem(key)  | Remove an item by key  |
| clear()  | Clear all storage  |


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
- http://react.tips/radio-buttons-in-reactjs/
- https://reactgo.com/tutorials/react/
- https://www.taniarascia.com/promise-all-with-async-await/
