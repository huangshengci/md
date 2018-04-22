#PHP方向第一个半月阶段测试

##选择题

1. 下面为块元素的是( D )。
	* A. `<a href=""></a>`
	* B. `<em></em>`
	* C. `<span></span>`
	* **D. `<p></p>`**

2. 对display及visibility说明正确的是( C )。
	* A.`display及visibility都能实现隐藏，且执行效果一样`
	* B.`display及visibility都能实现隐藏，执行效果不一样，display保留原来的位置`
	* **C.`display及visibility都能实现隐藏，执行效果不一样，visibility保留原来的位置`**
	* D.`只有display实现元素隐藏`
3. 如何显示这样一个边框：上边框 10 像素、下边框 5 像素、左边框 20 像素、右边框 1 像素( B )。
	* A.`border-width:10px 5px 20px 1px`
	* **B.`border-width:10px 1px 5px 20px`**
 	* C.`border-width:20px 5px 10px 1px`
 	* D.`border-width:1px 20px 5px 10px`

4. 关于session与cookie的说法错误的是( C )。
	* A.`session与cookie都可以记录客户状态`
 	* B.`在设置session和cookie之前都不能输出`
 	* **C.`在使用cookie之前必须先使用cookie_start()函数初始`**
 	* D.`cookie是客户端技术，session是服务器端技术`

5. 以下PHP程序，要输出字符"C"，那么下划线处应填写的下标是( D )。
	```php
	<?php
		$arr = array(-8=>"A",-5=>"B","C","D"); 
		echo $arr[__];
	?> 
	```
	* A.`-4`
 	* B.`1`
 	* C.`2`
 	* **D.`0`** 

6. 如果不给cookie设置过期时间，那么cookie默认保存时间是( D )。
	* A.`立刻过期`
 	* B.`永不过期`
 	* C.`cookie无法设置`
 	* **D.`在浏览器会话结束时过期`**

7. 下面PHP程序的输出结果是( A )。
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
	* **A.`Array (13,27,38,49,65,76,97)`**
 	* B.`Array (97,76,65,49,38,27,13)`
 	* C.`Array (97,76,65,13,27,38,49)`
 	* D.`Array (97,76,65,49,38,27,13)`

8. 以下PHP程序的输出结果是( B )。
	```php
	<?php 
		$str = "substr"; 
		echo $str('tarena',-2,-1); 
	?>
	```
	* A.`substr('tarena',-2,-1)`
 	* **B.`n`**
 	* C.`a`
 	* D.`Fatal Error`

9. 以下PHP程序的输出结果是( D )。
	```php
	<?php 
		$str = "3.5sw"; 
		echo $str + 2; 
	?>
	```
	* A.`2`
 	* B.`3`
 	* C.`3.5`
 	* **D.`5.5`**

10. 以下PHP程序的输出结果是( A )。
	```php
	<?php 
		$i = 5; 
		$n = &$i; 
		unset($i); 
		echo $n; 
	?>
	```
	* **A.`5`**
 	* B.`null`
 	* C.`""`
 	* D.`0`

11. 以下PHP程序的输出结果是( C )。 
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
	* **C.`true,7,1`**
	* D.`6,7,10`

12. 以下PHP程序的输出结果是( B )。
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
	* **B.`-1,3`**
	* C.`4,1`
	* D.`1,4`

13. 样式优先级说明正确的是( B )。
	* A.`行内样式优先级最高，标签选择器样式优先级最低`
	* **B.`Id选择器高于类别选择器高于标签选择器`**
	* C.`群组选择器最高`
	* D.派`生选择器高于群组选择器`

14. ```<?php echo count(strlen("http://php.net")); ?>```的执行结果是( C )？
	* A.`空白`
	* B.`0`
	* **C.`1`**
	* D.`2`

15. 以下PHP程序的输出结果是( A )。 
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
	* **A.`3 2 1 0 1 2`**
	* B.`3 2 1 0 -1 1 2`
	* C.`3 2 1 0 1 2 3`
	* D.`3 2 1 0 -1 1 2 3`

16. `$str='123a45b';$num=(int)$str;` 变量 `$num` 中的值是多少( B )？
	* A.`0`
	* **B.`123`**
	* C.`12345`
	* D.`45`

17. (**多选**)PHP中以下哪些情况会产生短路情况( BD )。
	* A.`&&或or运算时，第一个表达式的结果为true`
	* **B.`&&或and运算时，第一个表达式的结果为false`**
	* C.`||或and运算时，第一个表达式为true`
	* **D.`||或or运算时，第一个表达式为true`**

18. (**多选**)在PHP的字符数据类型中，单引号与双引号的区别有( ACD )。
	* **A.`双引号内的变量可以被PHP引擎正确解析`**
	* B.`单引号内的变量可以被PHP引擎正确解析`
	* **C.`双引号内的转义符可以被PHP引擎正确解析`**
	* **D.`单引号仅能识别\’与\\两个转义符`**

19. (**多选**)在MySQL数据库中，主键约束与唯一约束的区别有( BD )。
	* A.`主键列的数据类型不限，但此列必须是唯一并且非空`
	* **B.`一张数据表只能有一个主键`**
	* C.`唯一性约束所在的列允许空值`
	* **D.`数据表可以包含有多个唯一约束`**

20. (**多选**)MySQL中修改数据表的名字的命令是( AB )。
	* **A.`Alter table tablename rename to new_name`**
	* **B.`Alter table tablename rename new_name`**
	* C.`Rename tablename to newname`
	* D.`Rename tablename newname`

***

##简答题

1. PHP中魔术方法有哪几个？请举例说明各自的用法。
> 1、 __construct() ：实例化对象时自动调用。
> 2、 __destruct() ：销毁对象或脚本执行结束时自动调用。
> 3、 __call() ：调用对象不存在得方法时执行此函数。
> 4、 __get() ：获取对象不存在的属性时执行此函数。
> 5、 __set() ：设置对象不存在的属性时执行此函数。
> 6、 __isset() : 检测对象的某个属性是否存在时执行此函数。
> 7、 __unset() ：销毁对象的某个属性时执行此函数。
> 8、 __toString() ：将对象当作字符串输出时执行此函数。
> 9、 __clone() ：克隆对象时执行此函数。
> 10、__autoload() ：实例化对象时，当类不存在时，执行此函数自动加载类。
> 11、__sleep() ：serialize之前被调用，可以指定要序列化的对象属性。
> 12、__wakeup ：unserialize之前被调用，可以执行对象的初始化工作。
> 13、__set_state() ：调用var_export时，被调用。用__set_state的返回值做为var_export的返回值。
> 14、__invoke() ：将对象当作函数来使用时执行此方法，通常不推荐这样做。

2. cookie与session的区别?
> 1、cookie数据存放在客户的浏览器上，session数据放在服务器上。
> 2、cookie不是很安全，别人可以分析存放在本地的COOKIE并进行COOKIE欺骗
	 考虑到安全应当使用session。
> 3、session会在一定时间内保存在服务器上。当访问增多，会比较占用你服务器的性能
	 考虑到减轻服务器性能方面，应当使用COOKIE。
> 4、单个cookie保存的数据不能超过4K，很多浏览器都限制一个站点最多保存20个cookie。
> 5、所以个人建议：
    将登陆信息等重要信息存放为SESSION
    其他信息如果需要保留，可以放在COOKIE中
    
3. 以下语句输出的结果是什么?
	```php
	$a = 3;
	echo "$a",'$a',"\\\$a","${a}","$a"."$a","$a"+"$a";
	```
	答 : 3$a\$a3336

4. 常用的超全局变量(8个)
> 1、 ```$_GET ----->get传送方式```
> 2、 ```$POST ----->post传送方式```
> 3、 ```$REQUEST ----->可以接收到get和post两种方式的值```
> 4、 ```$GLOBALS ----->所有的变量都放在里面```
> 5、 ```$FILE ----->上传文件使用```
> 6、 ```$SERVER ----->系统环境变量```
> 7、 ```$SESSION ----->会话控制的时候会用到```
> 8、 ```$COOKIE ----->会话控制的时候会用到```

5. 语句include和require的区别是什么？为避免多次包含同一文件，可以用(?)语句代替他们
> 1、 require是无条件包含，也就是如果一个流程里加入require，无论条件成立与否都会先执行require，当文件不存在或者无法打开的时候，会提示错误，并且会终止程序执行
> 2、 include有返回值，而require没有(可能因为如此require的速度比include快)，如果被包含的文件不存在的化，那么会提示一个错误，但是程序会继续执行下去
注意:包含文件不存在或者语法错误的时候require是致命的，而include不是
> 3、 require_once表示了只包含一次，避免了重复包含

6. @test()和&test()的区别?
> 1、 @test()的作用是屏蔽test()方法中警告的作用 
> 2、 &test()引用test()方法

7. 表单中get和post提交方式的区别?
> 1、 get是把参数数据队列加到提交表单的action属性所指的url中，值和表单内各个字段一一对应，从url中可以看到
	  post是通过HTTPPOST机制，将表单内各个字段与其内容防止在HTML的head中一起传送到action属性所指的url地址，用户看不到这个过程
> 2、 对于get方式，服务器端用Request.QueryString获取变量的值
	  对于post方式，服务器端用Request.Form获取提交的数据
> 3、 get传送的数据量较小，
	  post传送的数据量较大，一般被默认不受限制，但在理论上，IIS4中最大量为80kb，IIS5中为1000k，
	  get安全性非常低，post安全性较高

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
	答 : 2 2 3 2 4 2

29. 请写出Apache安装和MySQL安装和启动的命令?
	答 : Apache : 安装 httpd -k install 启动 net start apache2.4
	Mysql : 安装 mysqld --install 启动 net start mysql

30. 怎么配置环境变量和为什么要配置环境变量?
	答 : 1、我的电脑右键->属性->高级系统设置->环境变量->系统变量->Path(双击)->粘贴程序的可执行文件的路径(一般是bin目录 **D:\Apache24\bin** | **D:\mysql5.7\bin** | **D:\php7.0**),最后加个英文的分号(;)->确定即可
	2、配置环境变量 是为了在DOS界面执行某个命令，系统无法在当前文件夹里找到对应的.exe，那么系统就会去path包含的路径找挨个找看是否能知道对应的.exe，一旦找到第一个对应的.exe就运行命令，其他的路径下就不找了。如果找不到你就会看到“系统找不到某某命令”的提示。






	
