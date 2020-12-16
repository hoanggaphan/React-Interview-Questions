
# Phỏng vấn React

## Nguồn tham khảo
* <a href="https://www.edureka.co/blog/interview-questions/react-interview-questions" target="_blank" rel="noopener noreferrer">edureka.co</a>
* <a href="https://www.simplilearn.com/tutorials/reactjs-tutorial/reactjs-interview-questions" target="_blank" rel="noopener noreferrer">simplilearn.com</a>

<a  id="top"></a>
## Mục lục

* [General React Interview Questions](#general_questions)

* [React Component Interview Questions](#component_questions)

* [React Redux Interview Questions](#redux_questions)

* [React Router Interview Question](#router_questions)

* [ReactJS Styling Interview Questions](#styling_questions)

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
1. Bất cứ khi nào bất kỳ dữ liệu cơ bản nào thay đổi, toàn bộ UI sẽ được hiển thị lại trong biểu diễn **Virtual DOM**. 
![Virtual DOM 1](https://cdn1.bbcode0.com/uploads/2020/12/16/589994042ba10554685a9d6315c24ac2-full.png)

2. Sau đó sự khác biệt giữa **Virtual DOM** mới và **Real DOM** trước đó được tính toán.
![Virtual DOM 2](https://cdn1.bbcode0.com/uploads/2020/12/16/e5f1a852eff1e4d623f133ef6ed4604b-full.png)

3. Sau khi tính toán xong, **Real DOM** sẽ chỉ được cập nhật với những thứ đã thực sự thay đổi.
![Virtual DOM 3](https://cdn1.bbcode0.com/uploads/2020/12/16/d46a52c7400b7b212755d3686585e2ff-full.png)
