# Timedoor Training Teen
## Intermediate A - Meeting 1

Pertemuan 1 mempelajari html dasar, hubungan antara html,css,js. Kita juga mengingatkan kemabli tentang variabel, array dan function melalui aplikasi changing color 

>https://timedoor-change-the-color.netlify.app/

Link Video
>Hello, World! Award Winning Short Film (Shot on GH4)
>>https://www.youtube.com/watch?v=egQH4vM1q1A



###  HTML Code Basic

```html
<body>
    <div class='center'>
        <h1 id='greeting'> Hello </h1>
        <h2>Let’s Change the Color</h2>
        <button> Click Me </button>
    </div>
</body>
```

### CSS Code Basic

```html
    <style>
        div {
            padding-top: 100px;
            text-align: center
        }

        button {
            background-color: red;
            color: white;
            text-align: center;
            font-size: 20px;
        }
    </style>
```
### Javascript Basic
```html
<script>
    //Initializing variables
    const button = document.querySelector('button')
    const body = document.querySelector('body')
    var name = prompt("What’s Your Name?")
    //Print variable value in HTML body 
    document.getElementById("greeting").innerHTML
        = "Hello " + name + "!";

    var colors = ['red', 'green', 'blue',
        'yellow', 'pink', 'purple', 'violet']
    body.style.backgroundColor = colors[0]

    function changeColor() {
        // choose random number from array colors
        var colorIndex = parseInt(Math.random() * colors.length)
        // set background to color Index
        body.style.backgroundColor = colors[colorIndex]
    }

    // when button clicked, call function changeColor
    button.addEventListener('click', changeColor)
</script>
```

## Challenge



###  HTML Code Challenge

```html
<body>
    <div class='center'>
        <h1 id='greeting'> Hello </h1>
        <h2>Let’s Change the Color</h2>
        <button> Click Me </button>
        <!-- Challenge -->
        <h1 id='text-color'></h1>
    </div>
</body>
```

### Javascript Challenge
```html
<script>
    //Initializing variables
    const button = document.querySelector('button')
    const body = document.querySelector('body')
    var name = prompt("What’s Your Name?")
    //Print variable value in HTML body 
    document.getElementById("greeting").innerHTML
        = "Hello " + name + "!";

    var colors = ['red', 'green', 'blue',
        'yellow', 'pink', 'purple', 'violet']
    body.style.backgroundColor = colors[0]

    function changeColor() {
        // choose random number from array colors
        var colorIndex = parseInt(Math.random() * colors.length)
        // set background to color Index
        body.style.backgroundColor = colors[colorIndex]
        // challenge
        document.getElementById("text-color").innerHTML = "this is " + colors[colorIndex];
    }

    // when button clicked, call function changeColor
    button.addEventListener('click', changeColor)
</script>
```

