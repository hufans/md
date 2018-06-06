**nodejs**
===
__2018年6月4日__
---
>*了解cookies 的用法熟悉cookies的参数。 对于中间件的熟悉，以及传入模块app.use(require("module"))作为中间件。以及中间件的推测实现。 了解了romens脚手架里面的用到的组件，大致看了一些组件的作用比如moment*

__2018年6月5日__
跨域
---
>*我们假设bob.com站点想要访问alice.com站点的某些数据。这种类型的请求由于浏览器的同源策略通常是不被允许的。不过，如果支持CORS请求，那么alice.com站点就可以通过增加一些特定的响应头信息来接受bob.com站点的数据访问* 
---
*res.end()参数必须是字符串*

---
>如何将nodejs 的异步变成同步
>module.export = cc , 默认构造函数
>export = func ,默认本身
>如果不指定文件夹，那么指定从 nodemodule文件夹带后缀名为文件，否则是文件夹（下的index.js文件）