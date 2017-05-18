### 事件绑定
addEventListener(type, listener, capture)

listener:

1. 一个函数(this指向当前响应事件的元素)
```javascript
var listener = function(event){};
document.body.addEventListener('click', listener);
```

2. 一个实现EventListener接口的对象(this指向该对象)
```javascript
function clickHandle(event) {
   // todo do something
}

var listener = {
    handleEvent: function(event) {
      var type = event.type;
      switch (type) {
          case 'click': 
              clickHandle(event);
              break;
          default:break;
      }
    }
};
document.body.addEventListener('click', listener);
```

    
