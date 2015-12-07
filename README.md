# 项目说明
- drag+xhr为拖拽上传代码
- form+xhr为表单上传文件代码
- show-thumbnail为展示缩略图代码

### XMLHttpRequest 说明
- XMLHttpRequest.upload  监听上传进度事件
   一个XMLHttpRequestEventTarget事件监听可以加载在上面
- void open(
    DOMString method,
    DOMString url,
    optional boolean async,
    optional DOMString user,
    optional DOMString password
    );   
- void send();
  void send(ArrayBuffer data);
  void send(ArrayBufferView data);
  void send(Blob data);
  void send(Document data);
  void send(DOMString? data);
  void send(FormData data);    
### Events  
- onreadystatechange作为XMLHttpRequest的实例属性被所有的浏览器支持
- onload, onerror, onprogress

### 继承
 XMLHttpRequest的接口也能继承自XMLHttpRequestEventTarget的属性
### XMLHttpRequestEventTarget 提供的事件接口处理XMLHttpRequest.
* onabort    call when a request is aborted
* onerror    call when a request encounters an error
* onload     call when an HTTP request returns after successfully loading content.   
* onloadstart   called when the HTTP request first begins loading data.
* onprogress    called periodically with information about the progress of the request(周期执行)
* ontimeout     called this only happens if a timeout has been previously established by setting the value of the XMLHttpRequest object's timeout attribute
* onloadend    called when the load is completed, even if the request failed(xhr结束执行)
### 以上事件接口对FileReader同样适用
### [XHR参考](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest) 
### [FileReader参考](https://developer.mozilla.org/en-US/docs/Web/API/FileReader) 



# file-upload
