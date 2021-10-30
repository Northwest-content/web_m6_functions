`onClick` is the best way to let the styling code work when the button is closed 😎

**❓ Question:**

> Where do we write this magical `onClick`? And how will it know what code to activate?

**🤓 Answer:** 

> The answer is simple, you will need to connect the `onClick` to a `function` that has that specific code you wanna activate. `function`s are easy! 

![img](https://lh4.googleusercontent.com/AEVGnTvNXNfFyN9T2gLAAEbO6WvSjkY4tHBFVbUvGqyI05YvUGwViMWaeDWzBk4UZ_w1h-QH1nNacglESq6P3HQySyTk-XE25fVNGYCFN2lRVGfl757KyNv18YG323A5HU97L16b)

Let's put each code in a `function` 🔥

**Implementation:**

![img](https://lh3.googleusercontent.com/7fV82-2zc5IKA0s3mLxtt2cyOIh3-FiKSIRoWdhyORq36sh8fbosXyMis6HL9vDosmrX7y4AU6uJZsGD8Ve03OO_7ipCpo-xWz-YKlbNOnYoCabePEmIdanLg4BrM-n1M5ODuEu2)

``````javascript
//Dark mode code
function dark() { document.querySelector(".container").style.cssText = "background-color: black; color: white;" }
//Light mode code
function light() { document.querySelector(".container").style.cssText = "background-color: white; color: black;" }
``````

**❓ Question:**

> How will it know what code to activate the function? 

**🤓 Answer:** 

> By calling it 😇 try typing the function name outside:
>
> ![img](https://lh5.googleusercontent.com/iD4LYaN-h9aBZW7cF9p1ZgOgTxufp9K3XfRN4qPI2WF0mCCzup4P3_58B_1gVsL2V9JmMX_m8ucSHx5eBZBTJoQCWH6G9Fj2To6VLc2ypzV5MdB6-hg4sGtdj37UkR72eUzOLFzH)

**Fix ⚠:**

> Before you start pointing fingers that I lied to you!, I DID NOT LIE. You forgot to put the `()` next to the function name once you called it. 
>
> Try it now:
>
> ![img](https://lh3.googleusercontent.com/oBG1vrVBDq6XibEM5ruKV3gk7SGICfEJxRqysLrOLpPss9mPlDnDcDBR8xvjyrOIk01DrC7qwDd9JORhQKJMh47tf_b5dbwwg1s5fBhVdF2ujK4xOw0rczTB8eJZZtyStW9Pqygi)
>
> YES IT WORKED 😍

**❓ Question:**

> Where does the `onClick` come into action?

**🤓 Answer:** 

> Now our dear programmers! We will let the `onClick` call the `function`. The `onClick` needs to be in the button tag that does the calling:
>
> ![img](https://lh6.googleusercontent.com/l1TeUM1VadQO3X55Ct0mhXDrSAVlZpOHmqduNVutCfK2uJtblPvh0Bu9MU-uWN8RJbuKX_e8LxVcQcKsjX-ddGQKEuiKepFaU1V-QdsBoWfeoIQRSgMS0h_42cEspDuY1PF-6QBB)

````html
<div id="dark" onclick="dark()">Dark Mode</div>
<div id="light" onclick="light()">Light Mode</div>

````

**Output:**

![img](https://lh3.googleusercontent.com/SgPomWJN2Fp9X8HLN6_CreUuSsLcMwuDNK4eA7FODHfCV3lmfwbQPI8BjnAEYfcdjR0dR4Eq0GMvdbCISp72PVNKHLXkZYY-RS_5XXgaOmzL1p0vHpsA3jz76YtuTYNkXBqszlHE)

GREAT JOB 😍 `proud of you 👏🏻`