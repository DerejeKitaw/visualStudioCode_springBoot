# [Steps to generate and run spring boot application in visual studio code](https://www.youtube.com/watch?v=hxiWXe5oMrI&index=1&list=UUHzokwmJY7o_NrhrNybYWGw)
### 01_install Spring Boot Dashboard extension
### 02_install Java Extension Pack
### 03_Generate spring boot application
> 01_Command + P -> to open action bar for visual studio code

> 02_Type `>spring` 
* 01_Select Spring Initializer: Generate a Maven Project
* 02_Select Java
* 03_add your input Group Id for your project Eg. `come.dkitaw`
* 04_add Input Artifact Id for your project
* 05_Select Spring Boot version -> I will select 2.0.5 default one
* 06_add dependencies you need -> I will select DevTool and Web
* 07_[add actuator ops](https://spring.io/guides/gs/actuator-service/)
### 04_add server port ->I will use server.port=9898
### 05_Run application -> Should see error on the http://127.0.0.1:9898
### 06_Add "/hi" route
```js
@SpringBootApplication
@RestController
public class DemoApplication {

@GetMapping(value="/hello")
public String getMethodName() {
		return "Hello";
}
```
07_That is it!

