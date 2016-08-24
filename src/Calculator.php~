<?php
class Calculator {
    private $_val1 , $_val2;

    public function add($val){
        $result = 0;
        foreach($val as $value){
        $result += $value;
        }
        return $result;
    }

    public function subtract($val1,$val2){
   
        return $val1 - $val2;
    }

    public function multiply ($val){
   
        $result = 1;
        foreach($val as $value){
        $result *= $value;
        }
        return $result;
    }

    public function divide ($val1,$val2) {
        if($val2==0){
         
         throw new Exception('Error: Division by zero.');
         
        }
        return $val1 / $val2;
    }
}
$calculator = new Calculator();
try{
    unset($argv[0]);
    $action =array_shift($argv);
    if($action == 'add' || $action == 'sum') {
        echo $calculator->add($argv);
    } else if ($action == 'multiple') {
        echo $calculator->multiply($argv);
    }else if($action == 'subtract'){
        echo $calculator->subtract($argv[0],$argv[1]);
    } else if($action == 'divide'){
 
        echo $calculator->divide($argv[0],$argv[1]);
       
    }
}catch(Exception $e){
            echo $e->getMessage();
        }    

?>
