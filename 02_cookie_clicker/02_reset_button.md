Before writing more code in the`<script>` how about we export our `JavaScript`, because `JavaScript` is jealous that `HTML` has its own file and `CSS` has its own stylesheet. Now `JavaScript` needs its own `script` file: 

![img](https://lh6.googleusercontent.com/5z4kM8Gn4KU29tsfW0FVnLDpuHKpv3KWusNAZJHZuqqx7ExGyhfAVlWYbTLiL7GrAUzNq9vT-xE1Uj-tAe401Ux1I6avmFMc9fcJBPnBTjfQvIi_zz-aiYqbQeGo0eueBFZGi3_J)

Now like what we did with `CSS` we must add a bridge between them: ![img](https://lh5.googleusercontent.com/ObeMuRx7AfNUBu7YWvpgD5L1-xe-JOy_3Y_l9cagX1qCa17EzKU6tLUCQQReZB_NZ78ahJ_Z-1kxG5bypcn1Z13AqpzJcLBgcDB50CjxPpu_QpJjQn1H9VtjyUnQhpETiapXNOU8)Now Reset button: 

1. Create a `reset` function

   ![img](https://lh5.googleusercontent.com/gQ8P4qiHkj0C7Py0sUEthNcspIJzyfzuBDzt07yeI1qjBoh9upKXhzjW3LWSnRfJLfkCDOyTc1ZV9WWvsLgMVBp0F9FIcgLwOqQM6pj3IoHqHdZ9Iid2Op9zt4e2dpH8byA8jlO_)

2. Connect the `reset()` to the button using `onClick`

   ![img](https://lh6.googleusercontent.com/DpP8a3TI5LtjAPD0NFZxq5XXWJCUfLt4UEorvMU9rXLLK4_OCGvYJAku-IDtVkEFsOUkd9Jg9PPesjV-MPSMx3nE0r0GRaBDG_-RLXEuWTN1jkbL0uwxNQncZ5TV9xvzpBrDnDqd)

3. Set the `counter = 0` inside the `reset()` function

   ![img](https://lh3.googleusercontent.com/dRSgBfQK-_K_n1-WbqJPR8I6nAeJGXaMcVYKrWSbTAzUqQ2WBz2VidLu4cP6XfC3ClFRj9s9GTtmAkWhR4119jxaNw_U4Zu481_b0ckyKP-Nkj4wURvKrh3Y-yXDXGVtD3yc1shN)

``````html
<body class="container">
    <h1>Cookie Clicker Game</h1>
    <img src="cookie.png" alt="Cookie">
    <p id="value"></p>
    <div onclick="add()">ADD</div>
    <div onclick="reset()">Reset</div>
    <script src="script.js"></script>
</body>
``````

``````javascript
let counter = 0;
function add() {
  counter = counter + 1;
  document.querySelector("#value").innerHTML = counter;
}

function reset() {
  counter = 0;
}
``````

**Output:** 

![img](https://lh6.googleusercontent.com/TkdGyQcH076uqv-8nz1iOzG_P7uAKGulG2vUQ22IWeTxPnR5miBgHAYQ6cmuLljUvddib6imEDVl9trcS7PxECS1fa7HVqSgnVlclGbzQ-uvkHueeuad1HUbFTfrxe2DLzhhxLL7)

**Fix ⚠:**

> Do not forget to let the `innerHTML = counter`

![img](https://lh6.googleusercontent.com/R4QhjlE8oH36Q0cgwAB1TWL-bJo2tyJPGC29wrR653GgazRexa5TcneQDI7uHAN7NIEGINFy20XTOiGCM6gBRG0r0QSVrf16jPtbxAmBKbvze2Da4b40OtrS0tQU5TbwlniNrz2x)

Great JOB `proud of you 👏🏻`