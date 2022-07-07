# FKjsBaseLib
  FK肥客泉JS基础方法库
  
  * FKjsBaseLib v1.3.20220707
  * https://www.FK68.net
  * Copyright (c) 2019 Feikeq
  *
  * 时间：2009-03-08
  * 修改：2022-07-07
  * 作者：肥客泉 - [https://github.com/feikeq/](https://github.com/feikeq/)
  
  
  ## FKjsBaseLib API 使用文档：
  ### 安装
  ```html
  <script src="./FKjsBaseLib.min.js">＜/script>
  ```
  ### 使用
  ```javascript
  // 直接使用 $$FK$$ 变量像jQuery类似
  $$FK$$.ready(function(){
      // 在网页中所有DOM结构绘制加载完毕后就执行的函数。
  }
  ```
  
  ## 函数方法 function：
    -------------------------------------
  ```
    ver 查看当前JS库版本信息 
    isArray(obj) 判断是否为 Array 数组
    isObject(obj) 判断是否为 Object 对象
    trim(text) 去掉字符串前后空格
    JSON(obj||text)  将字符串转为JSON对象或将JSON转为字符串
    ready(fn) 在网页中所有DOM结构绘制加载完毕后就执行的函数
    getRootPath 获取网站根路径(站点及虚拟目录)，获得网站的根目录或虚拟目录的根地址
    getDomain 获取网站主域名根域名
    FKCookie(c_name, value, expireday, path, domain) Cookie操作，获取、设置、删除Cookie
    getCookieArray(text||null) 获取所有Cooike成为对象
    getParameterByName(name, url||null) 获取地址栏URL的参数{ name(必选) 为要得到的参数名 ,url(可选) 自定义地址或为空[当前网址]}
    getQueryString(url||null) 将URL地址里的params=value数据变成数组对象,url(可选) 自定义地址或为空[当前网址]}
    params(obj) 将JSON数组对象转成字符串参数 params 查询字符串 例 a=1&b=2
    addQueryString(query,url||null) 拼接地址链接URL的参数（检查 url 链接是否已经有参数，添加 ？问号 或 & 与号）
    serializeArray(formClass||formID) 实现form表单序列化的方法
    FKAjax(url, datas, method, callback, head) Ajax方法访问和操纵HTTP管道异步获取资源-自己动fetch或XMLHttpRequest
    realFormatSecond(time)  时间戳里的秒钟转为00:00格式
    timestamp2time(time) 时间字符串或时间戳转化成日期格式
    formatime(time,formatstr) 时间字符串或时间戳按指定方式进行格式化
    log(1,2,3...) 美化debug输出，与console.log差不多是打印输了出到控制台的简化命今
    copy(str) 复制文本到剪切版 成功:true 或 失败:false  执行完函数后，按ctrl + v试试
  ```
  
  ## $$FK$$的DOM操作function（可链式操作）：
    -------------------------------------
  ```
    (text) 通过CSS选择器获元素
    get(index) 获元素集合中的第几个
    html 设置被选元素的内容
    css 设置或返回被选元素的一个或多个样式属性
    hide 隐藏被选元素
    show(display) 如果被选元素已被隐藏则显示元素（非内联样式需要指定display 默认为 block ）
    attr(name,val) 设置或返回被选元素的属性值
    removeAttr(name) 从被选元素中移除属性
    removeClass(name) 从被选元素移除一个类
    addClass(name) 向被选元素添加一个类
    remove 移除被选元素包括所有的文本和子节点
    append(html) 向匹配元素集合中的每个元素结尾插入由参数指定的内容
    prepend(html) 向匹配元素集合中的每个元素开头插入由参数指定的内容
    after(html) 在匹配的元素之后插入内容
    before(html) 在每个匹配的元素之前插入内容
    each(function (index, ele){}) 遍历元素
    on(eventName, callback) 事件监听
  ```
