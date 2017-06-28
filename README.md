<?php
function array_random($arr, $num = 1){
shuffle($arr);
 
$r = array();
for ($i = 0; $i < $num; $i++) {
$r[] = $arr[$i];
}
return $num == 1 ? $r[0] : $r;
}
 
$a = array(
 
"\"MID \" ",
"\"SUP \" ",
"\"JGL \" ",
"\"ADC \" ",
"\"TOP \" ",
 
);
print_r(array_random($a));
?>
