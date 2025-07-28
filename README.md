# Spring Boot Demo Application

这是一个基础的 Spring Boot 应用程序，包含了基本的 Web 功能。

## 技术栈

- Spring Boot 3.2.0
- Java 17
- Maven
- Spring Web

## 快速开始

### 运行应用程序

```bash
# 使用 Maven 运行
mvn spring-boot:run

# 或者先编译再运行
mvn clean package
java -jar target/demo-0.0.1-SNAPSHOT.jar
```

### 访问应用

启动后，可以通过以下 URL 访问应用：

- 首页: http://localhost:8080/
- Hello 接口: http://localhost:8080/hello
- 带参数的 Hello 接口: http://localhost:8080/hello?name=YourName

## 项目结构

```
src/
├── main/
│   ├── java/
│   │   └── com/example/demo/
│   │       ├── DemoApplication.java
│   │       └── controller/
│   │           └── HelloController.java
│   └── resources/
│       └── application.yml
└── test/
    └── java/
        └── com/example/demo/
            └── DemoApplicationTests.java
```

## 开发

### 添加依赖

在 `pom.xml` 中添加所需的依赖项。

### 运行测试

```bash
mvn test
```

## 构建

```bash
mvn clean package
```

构建完成后，JAR 文件将位于 `target/` 目录中。
