# 1. Thế nào là JDK, JRE? Dùng JDK hoặc JRE trong những trường hợp nào?
JDK: Java Development Kit
JRE: Java Runtime Environment

JDK dùng để lập trình những ứng dụng java
JRE là môi trường để chạy các ứng dụng java

# 2. Các biến môi trường PATH và CLASSPATH là gì? và được ứng dụng trong thực tế (qua nhiều hệ điều hành Windows, Linux ...) như thế nào?

##PATH: Để chỉ ra đường dẫn của thư mục /bin của JDK
###Với Windows:
- Được đặt tại
 ![](http://image.prntscr.com/image/fe971ba8e5794f1ea5fea79bfb4153ab.png)
 
### Với Linux / MacOS:
- Được đặt trong /etc/profile hoặc ~/.bashrc hoặc ~/.bashprofile

##CLASSPATH: Để chi ra đường dẫn của các thư viện jar
###Với Windows khai báo trong system variable
  ```CLASSPATH=c:\Program Files\Java\jre1.8.0_121\lib\;.;
  ```
###Với Linux được khai báo tại /etc/profile hoặc ~/.bashrc hoặc ~/.bashprofile
```CLASSPATH=CLASSPATH=:/opt/jdk1.8.0_121/jre/lib:/opt/jdk1.8.0_121/jre/lib/ext:.
  export CLASSPATH
```
# 3. Làm thế nào chỉ cần 1 câu lệnh có thể thực thi 1 file chứa source java được soạn từ console hoặc notepad?
javac file_name.java && java file_name

# 4. Làm thế nào để tạo ra một bản protable JAVA có thể chạy mà không cần cài đặt? (đa phần các ứng dụng Java đều có yêu cầu cài sẵn môi trường Java)
