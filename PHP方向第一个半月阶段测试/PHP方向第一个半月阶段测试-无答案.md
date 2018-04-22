#PHP方向第一个半月阶段测试

##选择题

1. 下面为块元素的是(  )。
	* A. `<a href=""></a>`
	* B. `<em></em>`
	* C. `span></span>`
	* D. `<p></p>`

2. 对display及visibility说明正确的是(  )。
	* A.`display及visibility都能实现隐藏，且执行效果一样`
	* B.`display及visibility都能实现隐藏，执行效果不一样，display保留原来的位置`
	* C.`display及visibility都能实现隐藏，执行效果不一样，visibility保留原来的位置`
	* D.`只有display实现元素隐藏`
3. 如何显示这样一个边框：上边框 10 像素、下边框 5 像素、左边框 20 像素、右边框 1 像素(  )。
	* A.`border-width:10px 5px 20px 1px`
	* B.`border-width:10px 1px 5px 20px`
 	* C.`border-width:20px 5px 10px 1px`
 	* D.`border-width:1px 20px 5px 10px`

4. 关于session与cookie的说法错误的是(  )。
	* `A.session与cookie都可以记录客户状态`
 	* `B.在设置session和cookie之前都不能输出`
 	* `C.在使用cookie之前必须先使用cookie_start()函数初始`
 	* `D.cookie是客户端技术，session是服务器端技术`

5. 以下PHP程序，要输出字符"C"，那么下划线处应填写的下标是(  )。
	```php
	<?php
		$arr = array(-8=>"A",-5=>"B","C","D"); 
		echo $arr[__];
	?> 
	```
	* A.`-4`
 	* B.`1`
 	* C.`2`
 	* D.`0`

6. 如果不给cookie设置过期时间，那么cookie默认保存时间是(  )。
	* A.`立刻过期`
 	* B.`永不过期`
 	* C.`cookie无法设置`
 	* D.`在浏览器会话结束时过期`

7. 下面PHP程序的输出结果是(  )。
	```php
	<?php 
		function bubble_sort($array){ 
			$count = count($array); 
			if ($count <= 0) return false; 
			for($i=0; $i<$count; $i++){ 
				for($j=$count-1; $j>$i; $j--){ 
					if ($array[$j] < $array[$j-1]){ 
						$tmp = $array[$j]; 
						$array[$j] = $array[$j-1]; 
						$array[$j-1] = $tmp; 
					} 
				} 
			} 
			return $array; 
		} 
		$arr = array(49,38,65,97,76,13,27); 
		$arr = bubble_sort($arr); 
		print_r($arr); 
	?>
	```
	* A.`Array (13,27,38,49,65,76,97)`
 	* B.`Array (97,76,65,49,38,27,13)``
 	* C.`Array (97,76,65,13,27,38,49)`
 	* D.`Array (97,76,65,49,38,27,13)`

8. 以下PHP程序的输出结果是(  )。
	```php
	<?php 
		$str = "substr"; 
		echo $str('tarena',-2,-1); 
	?>
	```
	* `A.substr('tarena',-2,-1)`
 	* `B.n`
 	* `C.a`
 	* `D.Fatal Error`

9. 以下PHP程序的输出结果是(  )。
	```php
	<?php 
		$str = "3.5sw"; 
		echo $str + 2; 
	?>
	```
	* A.`2`
 	* B.`3`
 	* C.`3.5`
 	* D.`5.5`

10. 以下PHP程序的输出结果是(  )。
	```php
	<?php 
		$i = 5; 
		$n = &$i; 
		unset($i); 
		echo $n; 
	?>`
	```
	* A.`5`
 	* B.`null`
 	* C.`""`
 	* D.`0`

11. 以下PHP程序的输出结果是(  )。 
	```php
	<?php 
		$a=3; 
		$b=6; 
		$c=1; 
		if($a=5 || $b=7 && $c=10){ 
			$a++;  
			$b++; 
		} 
		var_dump($a,$b,$c); 
	?>
	```
	* A.`5,7,10`
	* B.`6,8,10`
	* C.`true,7,1`
	* D.`6,7,10`

12. 以下PHP程序的输出结果是(  )。
	```php
	<?php 
	$i = 3; 
	$n = 0; 
	if(--$n || ++$i){ 
		echo $n; 
		echo $i; 
	} 
	?>
	```
	* A.`0,3`
	* B.`-1,3`
	* C.`4,1`
	* D.`1,4`

13. 样式优先级说明正确的是(  )。
	* A.`行内样式优先级最高，标签选择器样式优先级最低`
	* B.`Id选择器高于类别选择器高于标签选择器`
	* C.`群组选择器最高`
	* D.`派生选择器高于群组选择器`

14. ```<?php echo count(strlen("http://php.net")); ?>```的执行结果是？
	* A.`空白`
	* B.`0`
	* C.`1`
	* D.`2`

15. 以下PHP程序的输出结果是(  )。 
	```php
	<?php 
	function Crawler($i){ 
		echo $i . '&nbsp;'; 
		$i--; 
		if($i>0){ 
			$fun = __FUNCTION__; 
			$fun($i); 
		} 
		echo $i . '<br/>'; 
	} 
	Crawler(3); 
	?>
	```
	* A.`3 2 1 0 1 2`
	* B.`3 2 1 0 -1 1 2`
	* C.`3 2 1 0 1 2 3`
	* D.`3 2 1 0 -1 1 2 3`

16. `$str='123a45b';$num=(int)$str;` 变量 `$num` 中的值是多少？
	* A.`0`
	* B.`123`
	* C.`12345`
	* D.`45`

17. (**多选**)PHP中以下哪些情况会产生短路情况(  )。
	* A.`&&或or运算时，第一个表达式的结果为true`
	* B.`&&或and运算时，第一个表达式的结果为false`
	* C.`||或and运算时，第一个表达式为true`
	* D.`||或or运算时，第一个表达式为true`

18. (**多选**)在PHP的字符数据类型中，单引号与双引号的区别有(  )。
	* A.`双引号内的变量可以被PHP引擎正确解析`
	* B.`单引号内的变量可以被PHP引擎正确解析`
	* C.`双引号内的转义符可以被PHP引擎正确解析`
	* D.`单引号仅能识别\’与\\两个转义符`

19. (**多选**)在MySQL数据库中，主键约束与唯一约束的区别有(  )。
	* A.`主键列的数据类型不限，但此列必须是唯一并且非空`
	* B.`一张数据表只能有一个主键`
	* C.`唯一性约束所在的列允许空值`
	* D.`数据表可以包含有多个唯一约束`

20. (**多选**)MySQL中修改数据表的名字的命令是(  )。
	* A.`Alter table tablename rename to new_name`
	* B.`Alter table tablename rename new_name`
	* C.`Rename tablename to newname`
	* D.`Rename tablename newname`

***

##简答题

1. PHP中魔术方法有哪几个？请举例说明各自的用法。
	答 :

2. cookie与session的区别?
	答 :

3. 以下语句输出的结果是什么?
	```php
	$a = 3;
	echo "$a",'$a',"\\\$a","${a}","$a"."$a","$a"+"$a";
	```
	答 : 

4. 常用的超全局变量(8个)
	答 : 

5. 语句include和require的区别是什么？为避免多次包含同一文件，可以用(?)语句代替他们
	答 : 

6. @test()和&test()的区别?
	答 : 

7. 表单中get和post提交方式的区别?
	答 : 

28. 请分别写出下列函数调用的结果
	```php
	<?php
	function fun1(){
		static $a=1;
		$a++;
		echo $a;
	}
	function fun2(){
		$b=1;
		$b++;
		echo $b;
	}
	fun1();
	fun2();
	fun1();
	fun2();
	fun1();
	fun2();
	?>
	```
	答 : 

29. 请写出Apache安装和MySQL安装和启动的命令?
	答 : Apache : 安装		启动
	Mysql : 安装		启动

30. 怎么配置环境变量和为什么要配置环境变量?
	答 : 






	
