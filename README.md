

# Phỏng vấn React

## Nguồn tham khảo
<a href="https://www.edureka.co/blog/interview-questions/react-interview-questions" target="_blank" rel="noopener noreferrer">edureka.co</a>

<a  id="top"></a>
## Mục lục

+ [General React Interview Questions](#general_questions)

+ [React Component Interview Questions](#component_questions)

+ [React Redux Interview Questions](#redux_questions)

+ [React Router Interview Question](#router_questions)

<a id="general_questions"></a>
## General React Interview Questions

**1. Differentiate between Real DOM and Virtual DOM.**
| **Real DOM** | **Virtual DOM** |
| --- | --- |
| 1. It updates slow. | 1. It updates faster. |
| 2. Can directly update HTML. | 2. Can’t directly update HTML. |
| 3. Creates a new DOM if element updates. | 3. Updates the JSX if element updates. |
| 4. DOM manipulation is very expensive. | 4. DOM manipulation is very easy. |
| 5. Too much of memory wastage. | 5. No memory wastage. |

**2. What is React?**
* React là 1 thư viện Javascript Front-End được phát triển bởi facebook vào năm 2011.
* Nó tuân theo cách tiếp cận **Component** giúp xây dựng các thành phần UI có thể tái sử dụng.
* Nó được sử dụng để xây dựng các Web và Mobile UI phức tạp và giàu tính tương tác.
* Mặc dù chỉ mới open-sourced vào năm 2015 nhưng, nó có 1 trong những cộng đồng lốn nhất hỗ trợ nó.

**3. What are the features of React?**
| Features | Description |
|---|---|
| **JSX** | JSX là cú pháp mở rộng của javascript. Nó được sử dụng với React để mô tả giao diện người dùng trông như thế nào. Bằng cách sử dụng JSX chúng ta có thể viết HTML trong javascript. |
| **Components** | Components là các thành phần nền tảng của bất kì ứng dụng React nào và 1 ứng dụng đơn lẻ thường bao gồm nhiều component. Component chia giao diện người dùng thành các phần độc lập, có thể tái sử dụng và xử lí riêng biệt. |
| **Virtual DOM** | React giữ một bản sao nhỏ gọn của **Real DOM** trong bộ nhớ và đó được gọi là **Virtual DOM**. Khi trạng thái của một đối tượng thay đổi, **Virtual DOM** chỉ thay đổi đối tượng đó trong **Real DOM**, thay vì cập nhật tất cả các đối tượng. |
| **One-way data-binding** | Liên kết dữ liệu 1 chiều giữ cho mọi thứ theo module và nhanh chóng. Luồng dữ liệu 1 chiều có nghĩa là khi thiết kế 1 ứng dụng React, bạn thường lồng các thành phần con trong các thành phần mẹ. |
| **High performance** | React chỉ cập nhật những component đã thay đổi, thay vì cập nhật tất cả các component cùng một lúc. Điều này dẫn đến các ứng dụng web nhanh hơn nhiều. |
| **Debugging** | Các ứng dụng React rất dễ kiểm tra do có một cộng đồng developer lớn. Facebook thậm chí còn cung cấp một [browser extension](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi) nhỏ giúp gỡ lỗi React nhanh chóng và dễ dàng hơn. |

**4. List some of the major advantages of React.**
* Tăng hiệu suất của ứng dụng.
* Nó có thể sử dụng trên cả client và server side (ssr).
* Tăng khả năng đọc mã với JSX.
* React dễ dàng tích hợp với khác framework khác như Meteor, Angular, ...
* Viết các UI test case trở nên cực kỳ dễ dàng

**5. What are the limitions of React**
* React là 1 library, ko phải framework nên ta sẽ cần kết hợp với nhiều library khác.
* Do có nhiều lựa chọn library, nên việc kết hợp với các thư viện khác sẽ mất thời gian để hiểu và học.
* Có thể khó hiểu đối với các lập trình viên mới bắt đầu.
* Việc code sẽ trở nên phức tạp hơn vì nó sử dụng **Inline Styles** và **JSX**.

**6. What is JSX?**\
JSX (JavaScript XML_) là một loại cú pháp mở rộng dành cho ngôn ngữ JavaScript viết theo kiểu XML. JSX cung cấp cú pháp ngọt (syntactic sugar) để thay cho câu lệnh  `React.createElement()`  trong React.

Mã lệnh viết bằng JSX sẽ được chuyển sang JavaScript để trình duyệt có thể hiểu được, ví dụ:
```JS
  render() {
    return(
      <div>
        <h1>Hello World!</h1>
      </div>
    );
  }
```

**7. what do you understand by Virtual DOM? giải thích hoạt động của nó**\
**Virtual DOM** là một phiên bản thu nhỏ của **Real DOM**, có thể coi nó như một bản sao của **Real DOM**, mà việc cập nhập không gây ảnh hưởng tới **Real DOM**. Nó có tất cả các thuộc tính giống như object **Real DOM**, nhưng nó không có khả năng viết lên màn hình như **Real DOM**.

Các bước hoạt động:
1. Bất cứ khi nào bất kỳ dữ liệu cơ bản nào thay đổi, toàn bộ UI sẽ được hiển thị lại trong biểu diễn **Virtual DOM**. \
![Virtual DOM 1](https://cdn1.bbcode0.com/uploads/2020/12/16/589994042ba10554685a9d6315c24ac2-full.png)

2. Sau đó sự khác biệt giữa **Virtual DOM** mới và **Real DOM** trước đó được tính toán.\
![Virtual DOM 2](https://cdn1.bbcode0.com/uploads/2020/12/16/e5f1a852eff1e4d623f133ef6ed4604b-full.png)

3. Sau khi tính toán xong, **Real DOM** sẽ chỉ được cập nhật với những thứ đã thực sự thay đổi.\
![Virtual DOM 3](https://cdn1.bbcode0.com/uploads/2020/12/16/d46a52c7400b7b212755d3686585e2ff-full.png)

**8. Why can’t browsers read JSX?**\
Trình duyệt chỉ có thể đọc các đối tượng Javascript nhưng JSX không phải là đối tượng javascript thông thường. Do đó, để cho trình duyệt có thể đọc được Javascript, ta cần chuyển đổi tệp JSX thành đối tượng Javascript bằng cách sử dụng các trình biến đổi như **Babel**.

**9. How different is React’s ES6 syntax when compared to ES5?**
1. **require vs import**
	```JS
	// ES5
	var React = require('react');

	// ES6
	import React from 'react';
	```
2. **export vs exports**
	```JS
	// ES5
	module.exports = Component;

	// ES6
	export default Component;
	```
3. **Component and function**
	```JS
	// ES5
    var MyComponent = React.createClass({
      render: function() {
	    return <h3>Hello World!</h3>;
      }
    });
    
    // ES6
    class MyComponent extends React.Component {
      render() {
	    return <h3>Hello World!</h3>;
      }
    }
	```
4. **Props**
	```JS
	// ES5
	var App = React.createClass({
	  propTypes: { name: React.PropTypes.string },
	    render: function() {
	      return <h3>Hello, {this.props.name}!</h3>;
	    }
	});

	// ES6
	class App extends React.Component {
	  render() {
	    return <h3>Hello, {this.props.name}!</h3>;
	  }
	}
	```
5. **State**
	```JS
	// ES5
	var App = React.createClass({
	  getInitialState: function() {
	    return { name: 'world'};
	  },
	  render: function() {
	    return <h3>Hello, {this.state.name}!</h3>;
	  }
	});

	// ES6

	class App extends React.Component {
	  constructor() {
	    super();
	    this.state = { name: 'world'};
	  }
	  
	  render() {
	    return <h3>Hello, {this.state.name}!</h3>;
	  }
	}
	```
**10. How is React different from Angular?**
| TOPIC | REACT | ANGULAR |
|--|--|--|
| ARCHITECTURE | Only the View of MVC | Complete MVC |
| RENDERING | Server-side rendering | Client-side rendering |
| DOM | Uses virtual DOM | Uses real DOM |
| DATA BINDING | One-way data binding | Two-way data binding |
| DEBUGGING | Compile time debugging | Runtime debugging |
| AUTHOR | Facebook | Google |

<a id="component_questions"></a>
## React Component Interview Questions

**11. What do you understand from “In React, everything is a component.”**\
Components là những thành phần xây dựng nên UI của ứng dụng React. Các Components chia toàn bộ giao diện người dùng thành các phần nhỏ độc lập và có thể tái sử dụng. Sau đó nó hiển thị các Components này độc lập với nhau mà ko ảnh hưởng đến phần còn lại của giao diện người dùng.

**12. Explain the purpose of  render()  in React.**
Mỗi component trong React phải có một phương thức render (). Nó trả về một element duy nhất là đại diện của DOM Component gốc. Nếu nhiều element HTML cần được hiển thị, chúng phải được nhóm lại với nhau bên trong một thẻ bao quanh như `<div></div>`, `<></>`, `<React.Fragment></React.Fragment>`.

**13.  How can you embed two or more components into one?**\
Chúng ta có thể nhúng nhiều component theo cách sau:
```JS
class MyComponent extends React.Component{
  render(){
    return(                 
      <div>
        <h1>Hello</h1>
        <Header/>
      </div>
    );
  }
}

class Header extends React.Component{
  render(){
    return
      <h1>Header Component</h1>
  };
}

ReactDOM.render(
  <MyComponent/>, document.getElementById('content')
);
```

**14.  What is Props?**\
Props là viết tắt của **Properties** trong React. Chúng là những thành phần chỉ có thể đọc, tức là bất biến. Chúng luôn được truyền từ các thành phần mẹ đến các thành phần con trong suốt ứng dụng. 1 thành phần con ko bao giờ có thể gửi **Props** trở về các thành phần mẹ. Điều này giúp duy trì luồng dữ liệu 1 chiều và thường dc sử dụng để render data động.

**15. What is a State in React and how is it used?**\
State là thành phần của 1 Component khác với Props được truyền từ bên ngoài vào.\
State là lưu lưu trữ các giá trị khởi tạo của component, khi state thay đổi thì component cũng được render lại.\
Ví dụ tạo, sử dụng và thay đổi state:
```JS
class App extends React.Component {
  constructor(props)  {
    super(props);
    this.state  =  {
      firstName:  "kid",
      lastName:  "kaito"
    };
  }

  changeName =  ()  =>  {
    this.setState({firstName:  "conan"});
    this.setState({lastName:  "edogawa"});
  }

  render() {
    return (
      <>
        <p>{this.state.lastName} - {this.state.firstName}</p>
        <button onClick={changeName}>Click</button>
      </>
    );
  }
}
```

**16. Differentiate between states and props.**
| Props | State |
|-------|-------|
| Props chỉ có thể đọc. | State có thể thay đổi bất đồng bộ.|
| Props là bất biến (immutable). | State thay đổi được (mutable).|
| Props cho phép truyền data từ 1 component đến component khác. | State giữ thông tin về component. |
| Props có thể truy cập bởi các component con. | State ko thể truy cập bởi các component con |
| Props được sử dụng để giao tiếp giữa các component. | States được sử dụng để render lại khi component thay đổi state. |
| Props làm component có thể tái sử dụng. | State ko thể làm component tái sử dụng. |
| Props được truyền từ bên ngoài vào và được kiểm soát ở nơi ta truyền vào. | State nằm bên trong nội bộ và được kiểm soát bởi chính component đó. |

**17. How can you update the state of a component?**\
Để update state ta sử dụng **this.setState()** trong React Class, **useState()** trong React Hook.
* **React Hook**
	```JS
	import React, { useState } from 'react';

	function Example() {
	  // count trả về bởi useState là giá trị khởi tạo ban đầu là 0.
	  // Sử dụng setCount trả về bởi useState để update state mới
	  const [count, setCount] = useState(0);
	  
	  return (
	    <div>
	      <p>You clicked {count} times</p>
	      <button onClick={() => setCount(count + 1)}>
	        Click me
	      </button>
	    </div>
	  );
	}
	```
* **React Classes**
	```JS
	import React, { useState } from 'react';
	
	class Example extends React.Component {
	  constructor(props) {
	    super(props);
	    this.state = {
	      count: 0
	    };
	  }

	  render() {
	    return (
	      <div>
	        <p>You clicked {this.state.count} times</p>
	        <button onClick={() => this.setState({ count: this.state.count + 1 })}>
	          Click me
	        </button>
	      </div>
	    );
	  }
	}
	```

**18. What is arrow function in React? How is it used?**\
**Arrow Function** là cú pháp ngắn gọn để viết 1 biểu thức hàm ko tên. Các function này cho phép liên kết đến ngữ cảnh của component 1 cách chính xác vì ES6 ko tự động liên kết. Các **Arrow Function** chủ yếu hữu ích khi làm việc với các higher order functions.
```JS
//General way
render() {
  return(
    <MyInput onChange={this.handleChange.bind(this)} />
  );
}

//With Arrow Function
render() {
  return(
    <MyInput onChange={(e) =>this.handleOnChange(e)} />
  );
}
```

**19. Differentiate between stateful and stateless components.**
| Stateful Component | Stateless Component |
|--|--|
| Còn gọi là Smart Component | Còn gọi là Dump Component |
| Thường khai báo các function handle event sau đó truyền xuống Stateless Component  | Thường nhận props và sau đó render ra UI cần thiết |
| Có state | Không có state |
| Có các Lifecycle Methods | Không có Lifecycle Methods |
 
 **20. What are the different phases of React component’s lifecycle?**\
Có 3 giai đoạn chính trong 1 vòng đời của component:
+ **Initial Rendering Phase:** Đây là giai đoạn component được khởi tạo và gắn vào DOM. 
+ **Updating Phase:** Giai đoạn cập nhật và re-render chỉ xảy ra khi Props hoặc State thay đổi.
+ **Unmounting Phase:** Giai đoạn cuối cùng, xảy ra khi component bị loại bỏ khỏi DOM.

 **21. Explain the lifecycle methods of React components in detail.**\
 1. **componentWillMount()** - được gọi trước khi quá trình gắn kết xảy ra.
 2. **componentDidMount()** - được gọi ngay sau khi một component được gắn kết
 3. **componentWillReceiveProps()** - được gọi trước khi 1 component được gắn kết nhận được các props mới.
 4. **shouldComponentUpdate()** - cho React biết có nên update khi state hoặc props thay đổi. return true nếu muốn update và ngược lại return false.
 5. **componentWillUpdate()** - được gọi trước khi rendering vào DOM.
 6. **componentDidUpdate()** - được gọi sau khi rendering vào DOM.
 7. **componentWillUnmount()**- được gọi khi 1 component loại bỏ khỏi DOM. Sử dụng để giải phóng bộ nhớ. 
 
 **22. What is an event in React?**\
Trong React, các event được kích hoạt khi như di chuột, nhấp chuột, nhấn phím, v.v. Xử lý các event này tương tự như xử lý các event trong DOM elements. Nhưng có một số khác biệt về cú pháp như:
+ Các sự kiện được đặt tên theo qui tắc camelCase.
+ Sự kiện được truyền dưới dạng fuction thay vì string.

**23. How do you create an event in React?**
```js
class Display extends React.Component({
  show(evt) {
    // do something
  },

  render() {
    // Render the div with an onClick prop (value is a function)
    return (
      <div onClick={this.show}>Click Me!</div>
    );
  }
});
```

**24. What are synthetic events in React?**\
**Synthetic events** là các đối tượng hoạt động như một trình bao bọc trình duyệt chéo xung quanh sự kiện gốc của trình duyệt. Chúng kết hợp hành vi của các trình duyệt khác nhau thành một API. Điều này được thực hiện để đảm bảo rằng các sự kiện hiển thị các thuộc tính nhất quán trên các trình duyệt khác nhau.

**25. What do you understand by refs in React?**\
Refs là viết tắt của References trong React. Nó là một thuộc tính giúp lưu trữ một tham chiếu đến một element hoặc component trả về bởi render (). Chúng rất hữu ích khi chúng ta cần các phép đo DOM hoặc thêm các phương thức vào các component.
```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.myRef = React.createRef();  
  }
  
  render() {
    return <div ref={this.myRef} />;  
  }
}
```
> **Chú ý**: Refs không thể dùng với stateless component.

**26. List some of the cases when you should use Refs.**
+ Khi cần quản lí focus, select text hoặc phát lại media.
+ Kích hoạt các animations bắt buộc.
+ Tích hợp với thư viện DOM bên ngoài.

**27. How do you modularize code in React?**\
Sử dụng import và export của ES6. Giúp việc viết component thành những file riêng biệt.
```js
//ChildComponent.jsx
export default class ChildComponent extends React.Component {
  render() {
    return(
      <div>
        <h1>This is a child component</h1>
      </div>
    );
  }
}

//ParentComponent.jsx
import ChildComponent from './childcomponent.js';

class ParentComponent extends React.Component {
  render() {
    return(
      <div>
        <App />
      </div>
    );
  }
}
```

**28. How  are forms created in React?**
React Forms tương tự như các HTML Forms. Nhưng trong React, ta quản lí dữ liệu đầu vào thông qua state và cập nhật dữ liệu bằng setState ().
```js
class NameForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = {value: ''};
  }

  handleChange = (event) => {    
    this.setState({value: event.target.value});  
  }
  
  handleSubmit = (event) => {
    alert('A name was submitted: ' + this.state.value);
    event.preventDefault();
  }

  render() {
    return (
      <form onSubmit={this.handleSubmit}>
        <label>
          Name:
          <input type="text" value={this.state.value} onChange={this.handleChange} />        
        </label>
        <input type="submit" value="Submit" />
      </form>
    );
  }
}
```

**29. What do you know about controlled and uncontrolled components?**\
+ **Controlled  Component**: Dữ liệu form được xử lí bởi React, dữ liệu giữ trong state và cập nhật bằng setState().
+ **Uncontrolled Component**: Dữ liệu form được xử lí bởi DOM, sử dụng **ref** để truy cập dữ liệu.

**30. What are Higher Order Components(HOC)?**\
Higher-order component (HOC) là một kỹ thuật nâng cao trong React để sử dụng lại logic của component. Cụ thể, HOC là một function nhận đầu vào là component và trả về một component mới

**31. What can you do with HOC?**
+ Tái sử dụng code, logic.
+ [Render High jacking](https://stackoverflow.com/questions/48144659/what-is-render-hijacking-in-react)
+ Thao tác với State và Props.

**32. What are Pure Components?**\
Pure Components hay Function Components, Stateless Components là cách nhanh nhất để viết 1 component dưới dạng 1 function. Các component này nâng cao tính đơn giản của mã và hiệu suất của ứng dụng.

**33. What is the significance of keys in React?**\
Keys giúp React xác định những item đã thay đổi, được thêm vào hoặc bị xóa. Keys phải được cấp cho các phần tử bên trong mảng để cung cấp một danh tính ổn định.

<a id="redux_questions"></a>
## React Redux – React Interview Questions
**34. What were the major problems with MVC framework?**
+ Quản lí DOM rất tốn kém.
+ Ứng dụng chậm và không hiệu quả.
+ Sự lãng phí bộ nhớ lớn.
+ Luồng dữ liệu theo 2 chiều nên khó debug.

**35. Explain Flux.**\
Flux là một mẫu kiến trúc thực thi luồng dữ liệu đơn hướng. Nó kiểm soát dữ liệu có nguồn gốc và cho phép giao tiếp giữa nhiều component bằng cách sử dụng store trung tâm có quyền đối với tất cả dữ liệu. Mọi cập nhật dữ liệu trong toàn bộ ứng dụng chỉ được thực hiện tại đây. Flux cung cấp sự ổn định cho ứng dụng và giảm lỗi thời gian chạy.
![enter image description here](https://cdn1.bbcode0.com/uploads/2021/1/7/f90fce065c6c0348b294b717db9a68a5-full.png)

**36. What is Redux?**\
Redux là một trong những thư viện phổ biến nhất để phát triển front-end trên thị trường ngày nay. Nó là một vùng chứa trạng thái có thể dự đoán được cho các ứng dụng JavaScript và được sử dụng để quản lý trạng thái toàn bộ ứng dụng. Các ứng dụng được phát triển bằng Redux rất dễ kiểm tra và có thể chạy trong các môi trường khác nhau cho thấy hành vi nhất quán.

**37. What are the three principles that Redux follows?**
+ **Single source of truth:** State của toàn bộ ứng dụng được lưu trữ trong một cây object / state trong một store duy nhất. Cây state duy nhất giúp theo dõi các thay đổi theo thời gian và gỡ lỗi hoặc kiểm tra ứng dụng dễ dàng hơn.
+ **State is read-only:** Cách duy nhất để thay đổi state là kích hoạt một action. Một action là một object JS đơn giản mô tả sự thay đổi. Giống như state là đại diện tối thiểu của dữ liệu, action là đại diện tối thiểu của sự thay đổi đối với dữ liệu đó.
+ **Changes are made with pure functions:** Để chỉ định cách cây state được chuyển đổi bởi các action, bạn cần các pure functions. Các pure functions là những func có giá trị trả về phụ thuộc vào giá trị của các đối số của chúng.

**38. What do you understand by “Single source of truth”?**\
Redux sử dụng "Store" để lưu trữ toàn bộ trạng thái của ứng dụng tại một nơi. Vì vậy, tất cả trạng thái của component được lưu trữ trong store và chúng nhận được các bản cập nhật từ chính store. Cây state duy nhất giúp theo dõi các thay đổi theo thời gian và gỡ lỗi hoặc kiểm tra ứng dụng dễ dàng hơn.

**39. List down the components of Redux.**
+ **Action** – Một object mô tả những gì đã xảy ra.
+ **Reducer** – Nơi quyết định state sẽ thay đổi như thế nào.
+ **Store** – Cây state/object của toàn bộ app được lưu tại đây.
+ **View**  – Hiển thị data được cung cấp bởi store.
