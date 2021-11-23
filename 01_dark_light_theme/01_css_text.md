![img](https://lh4.googleusercontent.com/2yC1fWX9uQ4ZUPRgtKkGE5iS_PsiyVl5Ml8ZjwGVFLRQcrmBeD1BQr1N-ttDuEJAF5_U6M31YNbTr2dxxhZxxeZv1z9McwNHRXB4jzCQ_blIuXAr0CN7l8qLfhB5pk_VevzsBrc1)

This looks simple, right? Let's make it fun! 🔥

We will control the page style using the buttons

**Reminder:**

`document.querySelector().style` so let's see what can we do after `.style`:

| Command                                          | Output                      |
| ------------------------------------------------ | --------------------------- |
| `document.querySelector().style.backgroundColor` | Change the background color |
| `document.querySelector().style.color`           | Change the text color       |
| `document.querySelector().style.display`         | Change the displacement     |

And more, but what is we made it shorter

```javascript
document.querySelector().style.cssText = “..”
```

This looks much better, lets try it:

![img](https://lh6.googleusercontent.com/8VU1uWhQepSkZ0RDTfeNCEFKq-g4AI-14O2aRfQXKHvq_L-xUrxLvrCCLCT8fonop66TkFqBEP-tLoP8PRIUV-9xcJNQ0J4h3jQDJX_qbUX6tF5AyHpVld7e-ZSoQHJ36r7aFK2N)

```javascript
document.querySelector(".container").style.cssText = "background-color: black;";
```

We can add as much `css` as we want to know, on one condition! DO NOT forget the `;` between them

Now we got:

```javascript
//Dark mode code
document.querySelector(".container").style.cssText =
  "background-color: black; color: white;";
//Light mode code
document.querySelector(".container").style.cssText =
  "background-color: white; color: black;";
```

Now we only have to connect the buttons to this code 🤔
