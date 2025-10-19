<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>lindsay scientifique calculator</title>
    <link rel="stylesheet" href="style1.css">
</head>
<body>
    <div class="lindsay">
        <strong>LINDSAY SCIENTIFIC calculator</strong><br><br><br>
        <input type="text" id="display" disabled />
        <div class="buttons">
            <button onclick="clearDisplay()"><B>C</B></button>
            <button onclick="appendToDisplay('9')"><B>9</B></button>
            <button onclick="appendToDisplay('8')"><B>8</B></button>
            <button onclick="appendToDisplay('*')"><B>*</B></button>
            <button onclick="appendToDisplay('7')"><B>7</B></button>
            <button onclick="appendToDisplay('6')"><B>6</B></button>
            <button onclick="appendToDisplay('/')"><B>/</B></button>
            <button onclick="appendToDisplay('5')"><B>5</B></button>
            <button onclick="appendToDisplay('4')"><B>4</B></button>
            <button onclick="appendToDisplay('+')"><B>+</B></button>
            <button onclick="appendToDisplay('3')"><B>3</B></button>
            <button onclick="appendToDisplay('2')"><B>2</B></button>
            <button onclick="appendToDisplay('-')"><B>-</B></button>
            <button onclick="appendToDisplay('1')"><B>1</B></button>
            <button onclick="appendToDisplay('0')"><B>0</B></button>
            <button><a href="index1.html">mode scientific</a></button>
            <button onclick="appendToDisplay('.')"><B>.</B></button>
            <button onclick="calculateResult()"><B>=</B></button>
        </div>
        <p>"lindsay"</p>
    </div>
    <script src="script.js"></script>
</body>
</html>

<!DOCTYPE html>
<html>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CALCULATRICE SCIENTIFIQUE</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <div class="lindsay">
        <strong>LINDSAY scientific calculator</strong><br><br><br>
        <input type="text" id="display" disabled />
        <div class="buttons">
            <button onclick="clearDisplay()"><B>C</B></button>
            <button onclick="appendToDisplay('9')"><B>9</B></button>
            <button onclick="appendToDisplay('8')"><B>8</B></button>
            <button onclick="appendToDisplay('7')"><B>7</B></button>
            <button onclick="appendToDisplay('*')"><B>*</B></button>
            <button onclick="displayCurrentTime()"><B>Time</B></button>
            <button onclick="appendToDisplay('%')"><B>Mod</B></button>
            <button onclick="appendToDisplay('6')"><B>6</B></button>
            <button onclick="appendToDisplay('5')"><B>5</B></button>
            <button onclick="appendToDisplay('4')"><B>4</B></button>
            <button onclick="appendToDisplay('/')"><B>/</B></button>
            <button onclick="calculateSin()"><B>Sin</B></button>
            <button onclick="calculateLog()"><B>Log</B></button>
            <button onclick="appendToDisplay('3')"><B>3</B></button>
            <button onclick="appendToDisplay('2')"><B>2</B></button>
            <button onclick="appendToDisplay('1')"><B>1</B></button>
            <button onclick="appendToDisplay('+')"><B>+</B></button>
            <button onclick="calculateCos()"><B>Cos</B></button>
            <button onclick="calculateExp()"><B>Exp</B></button>
            <button onclick="calculatePower()"><B>^</B></button>
            <button onclick="appendToDisplay('0')"><B>0</B></button>
            <button onclick="appendToDisplay('.')">.</button>
            <button onclick="appendToDisplay('-')"><B>-</B></button>
            <button onclick="calculateTan()"><B>Tan</B></button>
            <button><a href="index.html">mode not <br> scientific</a></button>
            <button onclick="calculateFactorial()"><B>n!</B></button>
            <button onclick="convertToBinary()"><B>Bin</B></button>
            <button onclick="convertToHex()"><B>Hex</B></button>
            <button onclick="calculateSqrt()"><B>√</B></button>
            <button onclick="calculateResult()"><B>=</B></button>
        </div>
        <div class="conversion">
            <select id="conversionType">
                <option value="binary">Binaire</option>
                <option value="hexadecimal">Hexadécimal</option>
            </select>
            <button onclick="convertToDecimal()"><B>Dec</B></button><p>"lindsay"</p>
        </div>
    </div>    
    <script src="script1.js"></script>
</body>

</html>


body {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
.conversion {
    margin-top: 20px;
    display: flex;
    gap: 2%;
}

select {
    width: 135px;
    padding: 5px;
    font-size: 16px;
    height: 39px;
}
strong{
color: azure;
font-size: xx-large;
font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}
a{
    color: white;
    text-decoration: none;
}
.lindsay {
    background: black;
    border-radius: 12px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    padding: 20px;
    width: auto;
    border-style:ridge;
    height: auto;
}
B{
    font-size: 30px;
}
p{
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    color: white;
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    font-style:italic;
    margin-left: 15%;
}

#display {
    width: 100%;
    height: 60px;
    text-align: right;
    font-size: 50px;
    margin-bottom: 8px;
    padding: 5px;
    margin-left: -7px;
    border-radius: 5%;
    background-color: grey;
    color: black;
}

.buttons {
    display: grid;
    grid-template-columns: repeat(6, auto);
    gap: 15px;
    margin-top: 5%;
}

button {
    padding: 7px;
    font-size: 18px;
    cursor: pointer;
    border: none;
    background-color: #007BFF;
    color: white;
    border-radius: 5px;
    transition: background 0.3s;
}

button:hover {
    background-color: #0056b3;
}
@media screen and (min-width: 320px) and (max-width:1024px) {
    
    #display{
        height: 10%;
        margin-top: -15px;
        font-size: 23px;
    }
    
    strong{
        font-size: 60%;
    }
    .lindsay {
        background: black;
        width: auto;
        height: auto;
    }
    button {
        padding: 0.1px;
        font-size: 18px;
        cursor: pointer;
        border: none;
        background-color: #007BFF;
        color: white;
        border-radius: 5px;
        transition: background 0.3s;
        width: auto;
        height: auto;
    }
    .buttons{
        margin-left: -5px;
        gap: -3px;
        grid-template-columns: repeat(4, auto);
    }
    a{
        color: white;
    }
    button:hover {
        background-color: #0056b3;
    }
    p{
        font-size: 50%;
    }
}
@media screen and (min-width: 300px) and (max-width:1024px) {
    #display{
        height: auto;
        margin-top: -15px;
        font-size: 22px;
    }
    .buttons{
        margin-left: -5px;
        gap: -3px;
    }
    .lindsay {
        background: black;
        width: auto;
        height: auto;
    }
    @media screen and (min-width: 20px) and (max-width:1500px) {
        .lindsay {
            background: black;
            width: auto;
            height: auto;
        }
        .buttons{
            margin-left: -5px;
            gap: -3px;
        }
    }
}    

.block{
    display: none;
}


body {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-repeat: no repeat;
}
a{
    color: white;
    text-decoration: none;
}

strong{
color: azure;
font-size: x-large;
font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}

.lindsay {
    background: black;
    border-radius: 12px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    padding: 20px;
    width: 30%;
    border-style:ridge;
    height: auto;
}
B{
    font-size: 30px;
}
p{
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    color: white;
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    font-style:italic;
    margin-left: 30%;
}

#display {
    width: 100%;
    height: 60px;
    text-align: right;
    font-size: 50px;
    margin-bottom: 8px;
    padding: 5px;
    margin-left: -7px;
    border-radius: 5%;
    background-color: grey;
    color: black;
}

.buttons {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    margin-top: 5%;
}

button {
    padding: 5px;
    font-size: 18px;
    cursor: pointer;
    border: none;
    background-color: #007BFF;
    color: white;
    border-radius: 5px;
    transition: background 0.3s;
}

button:hover {
    background-color: #0056b3;
}
@media screen and (min-width: 320px) and (max-width:1024px) {
    
    #display{
        height: 10%;
        margin-top: -15px;
        font-size: 23px;
    }
    
    strong{
        font-size: 60%;
    }
    .lindsay {
        background: black;
        width: 30%;
        height: 41%;
    }
    button {
        padding: 0.1px;
        font-size: 18px;
        cursor: pointer;
        border: none;
        background-color: #007BFF;
        color: white;
        border-radius: 5px;
        transition: background 0.3s;
        width: 100%;
        height: 95%;
    }
    .buttons{
        margin-left: -5px;
    }
    
    button:hover {
        background-color: #0056b3;
    }
    p{
        font-size: 50%;
    }
}
@media screen and (min-width: 300px) and (max-width:1024px) {
    #display{
        height: 10%;
        margin-top: -15px;
        font-size: 22px;
    }
    .lindsay {
        background: black;
        width: 30%;
        height: 38%;
    }
    @media screen and (min-width: 20px) and (max-width:1500px) {
        .lindsay {
            background: black;
            width: 50%;
            height: auto;
        }
    }
}    


function appendToDisplay(value: string) {
    const display = document.getElementById('display') as HTMLInputElement;
    display.value += value;
}

function clearDisplay() {
    const display = document.getElementById('display') as HTMLInputElement;
    display.value = '';
}

function calculateResult() {
    const display = document.getElementById('display') as HTMLInputElement;
    try {
        display.value = eval(display.value).toString();
    } catch {
        display.value = 'syntax error';
    }
}


function appendToDisplay(value: string) {
    const display = document.getElementById('display') as HTMLInputElement;
    display.value += value;
}

function clearDisplay() {
    const display = document.getElementById('display') as HTMLInputElement;
    display.value = '';
}


function calculateResult() {
    const display = document.getElementById('display') as HTMLInputElement;
    try {
        display.value = eval(display.value).toString();
    } catch(error) {
        display.value = 'syntax error';
    }
}

function calculatePower() {
    const display = document.getElementById('display') as HTMLInputElement;
    const base = parseFloat(display.value);
    const exponent = prompt("Entrez l'exposant :");
    if (exponent !== null) {
        display.value = Math.pow(base, parseFloat(exponent)).toString();
    }
}

function calculateFactorial() {
    const display = document.getElementById('display') as HTMLInputElement;
    const num = parseInt(display.value);
    if (num < 0) {
        display.value = 'syntax error';
        return;
    }
    display.value = factorial(num).toString();
}

function factorial(n: number): number {
    return n <= 1 ? 1 : n * factorial(n - 1);
}

function calculateSqrt() {
    const display = document.getElementById('display') as HTMLInputElement;
    const num = parseFloat(display.value);
    display.value = Math.sqrt(num).toString();
}

function calculateLog() {
    const display = document.getElementById('display') as HTMLInputElement;
    const num = parseFloat(display.value);
    display.value = Math.log(num).toString();
}

function calculateExp() {
    const display = document.getElementById('display') as HTMLInputElement;
    const num = parseFloat(display.value);
    display.value = Math.exp(num).toString();
}

function calculateSin() {
    const display = document.getElementById('display') as HTMLInputElement;
    const num = parseFloat(display.value);
    display.value = Math.sin(num*Math.PI/180).toString();
}

function calculateCos() {
    const display = document.getElementById('display') as HTMLInputElement;
    const num = parseFloat(display.value);
    display.value = Math.cos(num*Math.PI/180).toString();
}

function calculateTan() {
    const display = document.getElementById('display') as HTMLInputElement;
    const num = parseFloat(display.value);
    display.value = Math.tan(num*Math.PI/180).toString();
}

function convertToBinary() {
    const display = document.getElementById('display') as HTMLInputElement;
    const num = parseInt(display.value);
    display.value = num.toString(2);
}

function convertToHex() {
    const display = document.getElementById('display') as HTMLInputElement;
    const num = parseInt(display.value);
    display.value = num.toString(16);
}
function displayCurrentTime() {
    const display = document.getElementById('display') as HTMLInputElement;
    const now = new Date();
    display.value = now.toLocaleTimeString();
}
function convertToDecimal() {
    const display = document.getElementById('display') as HTMLInputElement;
    const inputValue = display.value;
    const conversionType = (document.getElementById('conversionType') as HTMLSelectElement).value;
    let decimalValue: number;

    if (conversionType === 'binary') {
        decimalValue = parseInt(inputValue, 2);
    } else if (conversionType === 'hexadecimal') {
        decimalValue = parseInt(inputValue, 16);
    }

    if (!isNaN(decimalValue)) {
        display.value = decimalValue.toString();
    } else {
        display.value = 'Syntax error';
    }
}

