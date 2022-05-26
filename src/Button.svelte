<script>
    export let num = "";
    let series = ""

    function buttonPress1(){
        num += "1";
        return num;
    }
    function buttonPress2(){
        num += "2";
        return num;
    }
    function buttonPress3(){
        num += "3";
        return num;
    }
    function buttonPress4(){
        num += "4";
        return num;
    }
    function buttonPress5(){
        num += "5";
        return num;
    }
    function buttonPress6(){
        num += "6";
        return num;
    }
    function buttonPress7(){
        num += "7";
        return num;
    }
    function buttonPress8(){
        num += "8";
        return num;
    }
    function buttonPress9(){
        num += "9";
        return num;
    }
    function buttonPress0(){
        num += "0";
        return num;
    }
    function multiply() {
        num+= "*"
    }
    function add () {
        num+= "+"
    }
    function divide() {
        num += "/"
    }
    function subtract() {
        num += "-"
    }
    function calculate(){
        if(num.length<10){
        num = eval(num);} else {
            num = eval(num).toExponential();
        }
    }
    function buttonPress (number) {
        num += number
    }
    
    function deleteChar(){
        if(num != ""){
        let index = num.length-2;
        if(num.length<=1){
            num="";
        }
        else{
        let newstring = num[index];
        num = newstring;}}
    
    }
    function clear() {
        num = "";
    }
    

    
    </script>

<div>
    <span>
        <button on:click={buttonPress7}>7</button>
        <button on:click={buttonPress8}>8</button>
        <button on:click={buttonPress9}>9</button>
        <button on:click={clear}>C</button>
    </span>
</div>
<br>
<div>
    <span>
        <button on:click={buttonPress4}>4</button>
        <button on:click={buttonPress5}>5</button>
        <button on:click={buttonPress6}>6</button>
        <button on:click={add}>+</button>
    </span>
</div>
<br>
<div>
    <span>
        <button on:click={buttonPress1}>1</button>
        <button on:click={buttonPress2}>2</button>
        <button on:click={buttonPress3}>3</button>
        <button on:click={subtract}>-</button>
    </span>
</div>
<br>
<div>
    <span>
        <button on:click={buttonPress0}>0</button>
        <button on:click={calculate}>=</button>
        <button on:click={divide}>/</button>
        <button on:click={multiply}>x</button>
    </span>
</div>
<br>

<style>
    button {
  background-color: #add8e6;
  border: 0 solid #e2e8f0;
  border-radius: 1.5rem;
  box-sizing: border-box;
  color: #0d172a;
  cursor: pointer;
  display: inline-block;
  font-family: "Basier circle",-apple-system,system-ui,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";
  font-size: 1.1rem;
  font-weight: 600;
  line-height: 1;
  padding: 1rem 1.6rem;
  text-align: center;
  text-decoration: none #0d172a solid;
  text-decoration-thickness: auto;
  transition: all .1s cubic-bezier(.4, 0, .2, 1);
  box-shadow: 0px 1px 2px rgba(166, 175, 195, 0.25);
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  margin-right: 9px;
  margin-right: 9px;

}

button:hover {
    background-color: #2a2a72;
	background-image: linear-gradient(315deg, #2a2a72 0%, #009ffd 74%);
    color: white;
  
}

@media (min-width: 768px) {
  button {
    font-size: 1.125rem;
    padding: 1rem 2rem;
  }}
</style>

