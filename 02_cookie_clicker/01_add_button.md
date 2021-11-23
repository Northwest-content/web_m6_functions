This will be a short project, we will build a game 😍

![img](https://lh5.googleusercontent.com/9NdVfSPi38iwuGVGMEHjuwewd9wBp-Vt9OiVRe76IDdvg7qw62et7F7xCrczMzHsDr7qrFmDHxsK87Gkg39lx27DQH2KwSB8-7TkEp_3vlVKMBFt9C0Zoy0rrz1CqwRN7Ubwix-3)

LET'S START with the `ADD` button first

1. We need to create a variable called `counter` so the number of cookies can be displayed:

   ![img](https://lh5.googleusercontent.com/SXKaCw-aaM6VMxRfCLyVJ1ALVeAdxl6vyAeyCgvJSv8Ou1Mxvjs7CXPIEDS-TYQUsfZOqRcd2TFOEl6PsdqiVgD7cZ4nyLHoB2zT73eH0VP_UHqJGjNJzV8zYJy2q6YfJFpCUjAC)

   ```javascript
   let counter = 0;
   ```

2. Create `function add()`:

   ![img](https://lh3.googleusercontent.com/IadcsG8_4oR4Lwxn0XWrh_mojaafi1H3c8K6ErvijfqBtHSSdlUOkHCJDQXMydhb7yXiuq46eFO8eYu-D6XdSTbbyRevy2e2sz9R708-bFeog9x9kypWAiiAkJNtE6mYHfQ9IqcS)

   ```javascript
   function add() {}
   ```

3. Connect `add()` with the `ADD` button by `onClick`:

   ![img](https://lh3.googleusercontent.com/pPfQmsCq6_h6dxtboqv8RsYu0oQVatXimPGz3vbS07UDPkv0XBLNmFkCa1PRkKX_wQoL3SPRAqCCU7-OiEldXvm_z0h1n4W1Fq6Xrfo5r13b44gBYFoPW5SFo85JzADPJM30-uxt)

   ```html
   <div onclick="add()">ADD</div>
   ```

4. Write inside the function what the function needs to do

- Add `+1` to the `counter`:

  ![img](https://lh6.googleusercontent.com/80wW61EajNYmxvE1RYHypn0t_YPSNnAIxybw6UizFEmAFCQJiP-ox2CSQB-0waMGWM40xbPOUasCnsVcsWI9pXwGBEu0-iSfB-3B0a8w98t8lPyQggm_qjAQ_pEx3fMdiymocPzX)

  ```javascript
  function add() {
    counter = counter + 1;
  }
  ```

  **Note 📝:**

  > Why `counter = counter +1`? Because we are saying let `counter` equal `counter +1`, because we are assigning the `counter` with the prev `counter` value `+1`

- Display the `counter` value using `innerHTML`:

  ![img](https://lh3.googleusercontent.com/RsyhXN3Ri6e4rrht_aQCkE_ddIYNe-4G6SjIQDuCwVBLj4sMqJ-4prHLqNsEuHQ58S31lRmuqsjaIgqlHsGmv204dAhJTBBSZmgx72SGnDkWQy9ymeiVnogLkTPBg57_PEVhc0gi)

  ```javascript
  <script>
          let counter = 0;
          function add() {
              counter = counter + 1;
              document.querySelector("#value").innerHTML = counter;
          }
      </script>
  ```
