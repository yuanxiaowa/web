# toArray 将一个对象转化为数组

类似数组对象
> 就是长得像数组，但却不是数组的对象

以下是将这类对象转化为数组的方式

## [React](code/toArray--react.js)
1. 不能为数组，为对象或函数类型
2. `length`为数字类型
3. `length>0`时候得有`length-1`属性
4. 使用`Array.prototype.slice`把对象转化为数组
5. `ie<9`不支持slice，会抛异常。那么循环0到length-1，把对应值放在一个空数组里面

## [jquery](code/toArray--jquery.js)