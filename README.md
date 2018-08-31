# JS-Array-Function
数组的各种方法，一个JS的使用者，必须要清楚的。

``` bash
  var arr1 = [1,2,3,4,5,6,7];
  var arr2 = [11,22,33,44,55,66,77];
  var arr3 = [12,21,53,44,89,47];
  var arr4 = [87,54,54,58,63,87,12,45,55];
  
  var arrConcat = arr1.concat(arr2); /concat 数组链接起来
  console.log(arrConcat); //[1,2,3,4,5,6,7,11,22,33,44,55,66,77]
  
  var arrJoin = arr1.join("*"); //join把数组中的所有元素放入一个字符串
  console.log(arrJoin); //1*2*3*4*5*6*7
  
  var arrPop = arr1.Pop(); //pop删除数组中的最后一个元素，并返回这个元素，会改变元素的长度
  console.log(arrPop); // 7
  
  var arrPush = arr1.push("嘻嘻","哈哈"); //数组的末尾添加元素，并返回新的长度
  console.log(arrPush); //8
  
  var arrReverse = arr1.reverse(); //倒序数组的元素
  console.log(arrReverse); //["哈哈", "嘻嘻", 6, 5, 4, 3, 2, 1]
  
  var arrShift = arr1.shift(); //删除数组的第一个元素，并返回这个元素的值
  console.log(arrShift); //哈哈
  
  var arrSlice = arr1.slice(1,2); //方法从已有的数组返回选定的元素 slice(start,end);start规定从何处开始选取，end规定从何处结束选取 //此方法不会改   变数组的宽度，所以只是截取并没有删除，所以1是截取到6,是长度结束到6
  console.log(arrSlice);  //6
  
  var arrSort = arr3.sort();  顺序数组的元素
  console.log (arrSort);; // [12, 21, 44, 47, 53, 89]
  
  function sortNumber(a,b){ //排序函数，按数值大小排序，前端排序必备
    reutrn a - b
  };
  console.log(arr4.sort(sortNumber)); //[12, 45, 54, 54, 55, 58, 63, 87, 87]
  
  var arrSplice = arr1.splice(0,1,'splice'); //数组中添加/删除项目，返回被删除的项目; splice(index,howmany,item);index添加删除的位置，howmanysh删除的元素的数量,item添加的元素
  console.log(arrSplice); //["嘻嘻"]
  
  var arrTosoutce = arr1.toSourece(); //表示对象的源代码，只支持Gecko浏览器(火狐)
  console.log(arrTosoutce); //谷歌报错喽
  
  var arrTostring = arr1.toString(); //数组转化成字符串，并返回结果
  console.log(arrTostring); // splice,6,5,4,3,2,1
  
  var arrToLocalString = arr1.toLocaleString; //数组转化成本地字符串，并返回结果
  console.log(arrToLocalString); // splice,6,5,4,3,2,1
  
  var arrUnshift = arr1.unshift('unshift','shiftun'); //向数组开头添加一个或多个元素，并返回新的长度
  console.log(arrUnshift) // 9
  
  var arrValueOf = arr1.valueOf(); //返回原始对象，JS默认的方法;
  console.log(arrValueOf) // ["unshift", "shiftun", "splice", 6, 5, 4, 3, 2, 1]
  
```
> 上午弄得一半，半路叫去做VUE的懒加载去了，下午接着填，有点遗忘了一些，待我去买瓶生命一号。
