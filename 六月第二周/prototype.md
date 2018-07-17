# 原型链

>> 当我们声明一个js函数
    function Animal(){
        this.species = "Animal"; 
    }
>> 打印Animal 里面有几个属性 arguments,caller,length，name，以及 prototype，和 _/_proto__ 两个 可添加类型（为什么使用可添加类型这个词描述，后面解释）。

>> prototype 可扩充类型中有一个默认constructor 这个对象等于 Animal 本身。

>> var animlinstance = new Animal() 得到一个新的对象。
>> 对象中有两个属性，其中 __proto__ 中的 值是从 prototype中拷贝而来。所以这对对象保存了完整的 Animal

　　var Chinese = {
　　　　nation:'中国'
　　};

var Doctor ={
　　　　career:'医生'
　　}

function object(o) {
　　　　function F() {}
　　　　F.prototype = o;
　　　　return new F();
　　}

var Doctor = object(Chinese);


为什么js 的this比较难理解。
apply、call、bind比较
apply 、 call 、bind 三者都是用来改变函数的this对象的指向的；
apply 、 call 、bind 三者第一个参数都是this要指向的对象，也就是想指定的上下文；
apply 、 call 、bind 三者都可以利用后续参数传参；
bind 是返回对应函数，便于稍后调用；apply 、call 则是立即调用 。

this的指向在函数定义的时候是确定不了的，只有函数执行的时候才能确定this到底指向谁，实际上this的最终指向的是那个调用它的对象

如果返回值是一个对象，那么this指向的就是那个返回的对象，如果返回值不是一个对象那么this还是指向函数的实例。
 
function fn(){
    this.num = 1;
}
var a = new fn();
console.log(a.num); //1


 为什么this会指向a？首先new关键字会创建一个空的对象，然后会自动调用一个函数apply方法，将this指向这个空对象，这样的话函数内部的this就会被这个空的对象替代。

