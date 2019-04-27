## 零散知识点
### cookie
    在跨域请求中请求不到cookie
## 跨域
### 请求头
    Access-Control-Allow-Origin 只能设置一个域名 *所有的都能访问但是不允许使用
### 常用请求方式
请求方法|用处
---|---
get | 查
post | 增
put | 改
delete| 删
options| 探测请求，如果没问题请求
### JSONP
    1、Ajax对普通页面有跨域和权限问题,所有的页面和web服务都会存在跨域，不管任何东西只要有跨域就会不让请求
    2、但是有一些东西不会受跨域的影响，比如说有script,img,iframe这些标签都不会受跨域的影响
    3、jsonp可以用cb参数传递给服务端，服务端会将cb参数作为函数名用来包裹数据，这样客户端就会随意定义自己函数用来处理返回的数据