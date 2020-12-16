
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

