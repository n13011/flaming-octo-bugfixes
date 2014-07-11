<?php
	$sum = $_GET['sum'];
	if(ctype_digit($sum)){
		$kisuu = substr(decbin($sum), -1);
		if($sum % 2  == 0)
			print $sum .'=偶数だよ';
		else if($sum % 2 == 1)
			print $sum . '=奇数だよ';}
	else 
		print 'もじが混じってます';
?>
