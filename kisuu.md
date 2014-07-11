<?php
	//入力させたのをGETしてる
	$sum = $_GET['sum'];
	
	//入力させたのが数字だけか調べてる
	if(ctype_digit($sum)){
		
		//数字を２進数にして、１番後ろを見て０か１か判断してる
		$kisuu = substr(decbin($sum), -1);
	
		if($sum % 2  == 0)
			print $sum .'=偶数だよ';
		else if($sum % 2 == 1)
			print $sum . '=奇数だよ';}
	else 
		print 'もじが混じってます';
?>
