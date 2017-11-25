# Design Pattern - Factory Pattern
> Factory pattern là mẫu thiết kế được sử dụng nhiều nhất trong java. Loại design pattern này được tạo ra theo mô hình tạo mẫu như mẫu
> cung cấp một trong nhưng cách tốt nhất để tạo ra một đối tượng.
> Trong Factory pattern, chúng ta tạo đối tượng mà không phơi bày logic sáng tạo cho khách hàng và tham khảo các đối tượng mới được sử
> dụng một giao diện chung.
## Thực Hiện
Chúng ta tạo ra một interface Shape và các lớp cụ thể thực hiện giao diện shape. Một factory lớp ShapeFactory được định nghĩ trong bước tiếp theo. <br/>
FactoryPatternDemo, lớp demo của tối sẽ sử dụng ShapeFactory để lấy một đối tượng Shape. Nó sẽ pas thông tin (CIRCLE / RECTANGLE / SQUARE) để ShapeFactory lấy loại đối tượng nó cần.
![UMLFP](https://github.com/bigkizd/Design-Patern/blob/master/Factory%20Pattern/image/factory_pattern_uml_diagram.jpg)

### Step 1
Tạo một interface
``` java
public interface Shape{
  void draw();
}
```

