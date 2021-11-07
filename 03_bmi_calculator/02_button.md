Now we will do the `Get Result` button in steps: 

1. Create a `getBMI` function ( Notice how names are convenient)

   ![img](https://lh6.googleusercontent.com/SQgfvQMJ9vWBXPrkYGAgRoQ4R7mDduLnu9W7hJhBICHY0SHAe5YrHcejtsDDXAT6dxDs2x-pWYXecv7NvKI4yj2wlx1VxnncbqoywAquBxWn0c6qcstIACeDotrLzO01k5ELy90Q)

2. Use the `onClick` to call `getBMI`

![img](https://lh5.googleusercontent.com/tDVmR_eCijBgOLwMWHtaMviiC5YbCV-wu5fkSn9LL0-xbIFCLEHMRDpxfQHa0tulsRTScfSZbj44gL9_ufT8vlWpqbtC0NUM_ZZyX2Se287aPnSd0KQvXiEaqLletBhQAV5W_u1w)

3. Give each `input` an `id` to be able to call it

![img](https://lh5.googleusercontent.com/0IEHrzWWs64PNJ_qiduasTdsQagHXXuMRXZJi_OzbOLQKjzKhoGBsCBvVrHshlF-IX_-TlljhCK30qN60hFehf0a7Jptgr1SPsQej0in2CCubFT6UO9hiqxOGV0YHIBdNLESGnyn)

4. Collect the `height` and `weight` from the inputs 

   To be able to take a value we will say `document.querySelector().value`

![img](https://lh5.googleusercontent.com/s1sj_XIsTZ4iBnr7v0BRAz1JxiUHLXadGmiLRs2FcS18uLfcRHTdWLvEvIFPNvrpfoOAmIXihaNsDiBiW6U-1dkKTur2cYMS6SLAVvcsOvKWc-0mXAJgaPUaBqhNconSgjF6lfRm)

5. Do the calculation and save it in variable `result`

   Equation will be `result = w/(h*h)`
   
![img](https://lh6.googleusercontent.com/WCXeIpxjAogcK-AcWkGE59tZArCVMUgsjhRjWsOcr_XdZSNIRPJrky0WTEn_PRRtVUdEfQY37_kU-_L9lKRMA_ibqig38hvSCC8-8E4MAiSX9Tj4eHSBLTuC9OFr4xjmGQzBes8X)

6. Display result inside the `result` box

![img](https://lh4.googleusercontent.com/CkE3rJ3Ep5luVt9i7eUuuEBZwuiAsZrZ9HFPJAgIwsVjJbNTFg9L-YhqkliNQmfIHqimgYHrkJ9vDwpqQVhRMFAZDsI9ewT2gyM4JJr9pdpmgjpNdKFDBdV5oTJJfeIX8qN1XV6D)

   

**Output:** 

Let's compare our calculator to an online BMI calculator:![img](https://lh5.googleusercontent.com/7pSJT5oIjeWaZT6PH9emKE5rdeY8wGwUynDG0qatcf-15o6xFHYsL5S2fOYm6K_cKLr6Gm-WBD9KqZZEXAwYY7HdIYQClge0jCC_YhTvxt0UnrJMMEjtf4TiqJJQvvp8Tg5Znork)

**Fix ⚠:**

>  The reason for the simple difference in the result is multiplying the result with `1000`For the equation to be `(w / (h * h))*10000`:

![img](https://lh5.googleusercontent.com/HsUbMC7FiJupTgESHM9l8vUHLlQ1z_Jvli0cRAI60kLneIbt_Ik9_h8XXoEfYgBEFks3GaUzTU8T8c4SYCnVayFBEGsUBp-iaYWxJViqUGdJo3qexgKkvH82vONGGckZH5_QwA-O)

**Script:** 

````javascript
function getBMI() {
  let h = document.querySelector("#height").value;
  let w = document.querySelector("#weight").value;
  let result = (w / (h * h)) * 10000;
  document.querySelector("#result").innerHTML = result;
}
````

