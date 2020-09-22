<div align="center">

## Password Generator\.\.,


</div>

### Description

This function return Password consists of 0-9, a-z, A-Z
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Bhushan\-](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/bhushan.md)
**Level**          |Beginner
**User Rating**    |4.2 (79 globes from 19 users)
**Compatibility**  |PHP 3\.0
**Category**       |[Algorithims](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/algorithims__8-29.md)
**World**          |[PHP](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/php.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/bhushan-password-generator__8-733/archive/master.zip)





### Source Code

```
<?
 function PassGen() {
 $chars=array();
 for($i=48;$i<=57;$i++) {
	array_push($chars, chr($i));
 }
 for($i=65;$i<=90;$i++) {
	array_push($chars, chr($i));
 }
 for($i=97;$i<=122;$i++) {
	array_push($chars, chr($i));
 }
 while(list($k, $v)=each($chars)) {
  print $k." -> ".$v."<br>";
 }
 for($i=0;$i<8;$i++) {
	mt_srand((double)microtime()*1000000);
	$passwd.=$chars[mt_rand(0,count($chars))];
 }
 return $passwd;
}
 print PassGen();
```

