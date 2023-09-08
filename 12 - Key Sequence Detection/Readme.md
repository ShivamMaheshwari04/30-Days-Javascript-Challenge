**Day 12: Unleashing Hidden Magic with JavaScript**

On Day 12 of our 30 Days JavaScript Challenge, I uncovered a fascinating trick using event listeners and functions. Here's a quick breakdown:

🔮 **Magic with Key Events**: We began by creating an array called `pressed` to keep track of the keys pressed by the user. We also set up a `secretCode`, which is the combination of keys we want to detect. In our case, it's "shivam."

🔐 **Listening for Key Up**: We utilized the `window.addEventListener` method to listen for the "keyup" event, which fires when a key on the keyboard is released.

🧙‍♂️ **Magical Detection**: Inside the event listener function, we logged the key that was pressed (`e.key`) and added it to our `pressed` array. To keep the array's length in check, we used `pressed.splice` to remove older key entries if they exceed the length of our `secretCode`.

✨ **Unleashing the Magic**: Here comes the magic! We checked if the `pressed` array, when joined into a string, includes our `secretCode`. If the user types "shivam" consecutively, we get a "DING DING!" message logged to the console, and a fun function called `cornify_add()` is triggered to add some whimsical flair to the webpage.

🕵️‍♂️ **Observing the Process**: Throughout the process, we logged the content of the `pressed` array, allowing us to see the keys pressed and how our code operates.

This intriguing code allows us to create hidden easter eggs or interactive elements on websites. As we advance through our 30-day JavaScript journey, we'll continue to explore exciting JavaScript concepts and apply them in creative ways. Stay tuned for more enchanting discoveries ahead! 🪄✨