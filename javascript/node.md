## node module加载
1. node中的模块加载时单例的，即它会根据文件的绝对路径作为id来缓存模块
  (即module.exports引用的模块),同时意味着模块中的逻辑代码只会执行一次

    