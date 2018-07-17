>> resave : 是指每次请求都重新设置session cookie，假设你的cookie是10分钟过期，每次请求都会再设置10分钟 (时间到和每次访问重置时间)（用户输入密码）
>> saveUninitialized: 是指无论有没有session cookie，每次请求都设置个session cookie ，默认给个标示为 connect.sid (指定之前的sessionid失效)
>> 提交表单的问题
>> setTimeout问题