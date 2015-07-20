var http = require('http');
var fs = require('fs');
var async = require('async');
var server = http.createServer(function(req,res){
	//res.setHeader('Content-Length',body.length);
	res.setHeader('Content-Type','text/plain');
	res.write('hello!');
	console.log('you can do that byyourself~!');
	res.end();

});
 fs.readFile('./meng.txt','utf-8',function(err,data){
	console.log(data);
 });
//这是一个异步串行的调用的方式
async.series([function(callback){ 
	console.log('1');
	callback(null,"执行相关的代码");
},function(callback){  //callback 是总的Callback 执行的过程中传入相关的错误信息和结果内容 执行的先后的顺序
	console.log('3');
	callback(null,"你享受的很啊！");
	console.log('2');
}],function(err,result){
	console.log(result); //返回的结果是以数组的形式
});

//创建一个异步的并行执行的方式呢 如果是前面的函数中出现了错误，那后面的异步回调的部分将不能被执行了，只能等着
async.parallel([function(callback){
	console.log('one');
	callback(null,'mll');
},function(callback){
	console.log('two');
	callback('liuwendan','wendan');
}],function(error,content){
	console.log(error);
	console.log(content);
});

//前一个函数的执行结果，作为第二个函数的参数执行
async.waterfall([function(callback){
	console.log('这是神马样的代码啊');
	callback(null,'waterfall1');
},function(data,callback){ //回调函数的返回的结果作为作为第二个函数的参数传入，最终的结果是最后的回调函数执行的结果
	console.log(data+'--->');
	callback(null,'waterfall22');
}],function(error,data){
	console.log(data+'<----->');
});

//现在将要再次的实验async 的each的方法遍历只想相关的内容
var batada = [{'name':'zhangjing','age':'23'},{'name':'wendan','age':'34'},{'name':'fujing','age':'32'}];
async.each(batada,function(item,callback){
	console.log(item.age);
	console.log(item.name);
	callback(null);
},function(err){
	console.log(err); //难道这个只有错误的存在么，很难想象呢 each 的优先级高于流程控制的操作异步的操作
});

//async 主要实现了三个部分的流程控制功能
// 集合 Colllections 流程控制 Control Flow 工具类: Utils
// 集合的什么操作 map 操作
//依次的执行这代码里面的数据，然后保存到数组中
async.map(batada,function(item,callback){
	callback(null,item.name);
},function(err,data){
	console.log(data);
});
//实现过滤的参数的处理
async.filter(batada,function(item,callback){
	console.log(item);
	callback(item.name =='fujing'); //在满足条件的时候执行最后的回调函数，传递的数据是ITEM的内容
},function(data){
	console.log(data);
});
//异步的流程控制方面 concat 这个是有点不好操作了啊，那该怎么弄呢
//我们都是很难理解这个显示
server.listen(3000);
