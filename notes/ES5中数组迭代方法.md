# ES5中四种迭代数组的方法
> forEach(): 单纯的循环  
 
> some(): 当回调函数返回true时就停止循环
 
> findIndex(): 找到指定条件的元素的索引
 
> filter(): 过滤
    
 
 

## forEach()
- forEach循环数组的第一个参数为数组每一个的值，第二个为数组的索引，
并且会循环每一项，数组有几项就会循环几次；

		arr.forEach（（item,index）=> {
			console.log('我在循环' + index)
			if(条件表达式){
			
			}
		}）

## some()
- some循环数组的第一个参数为数组每一个的值，第二个为数组的索引，可使用return true提前终止循环：
	
		arr.some（（item,index）=> {
			console.log('我在循环' + index)
			if(条件表达式){
				
			retuen true
			}
		}）

## findIndex()
- findIndex循环数组，可使用return true终止遍历，同时返回该一项的索引
 
		arr.findIndex（item => {
			console.log('我在循环' + index)
			if(条件表达式){
				
			retuen true
			}
		}）

## filter()
- filter循环数组，可使用return true返回该项的值，但不会终止遍历，遍历所有项之后会统一返回一个包含所有满足条件的项的数组：

		arr.filter（item => {
			console.log('我在循环' + index)
			if(条件表达式){
				
			retuen true
			}
		}）
