**Day 15: Exploring Local Storage, Event Listeners, and Preventing Defaults in JavaScript**

On Day 15 of our 30 Days JavaScript Challenge, I dived into several essential JavaScript concepts. Here's a concise overview of what I learned:

📦 **Local Storage**: We began by harnessing the power of Local Storage in JavaScript. We utilized `localStorage.getItem()` to retrieve data stored in the browser's Local Storage. In this case, we fetched an array of items or created an empty one if it didn't exist using `JSON.parse()` and `localStorage.getItem('items')`.

📝 **Event Listeners**: We mastered the art of adding event listeners to HTML elements. The `addItems` element had a "submit" event listener attached to it, and the `itemsList` element was listening for "click" events. These event listeners allowed us to react to user interactions.

🚫 **Preventing Defaults**: To prevent the default behavior of a form submission (i.e., page reload), we learned to use `e.preventDefault()` within our `addItem` function. This allowed us to control the form submission and perform our desired actions without a page refresh.

📥 **Adding and Displaying Items**: Inside the `addItem` function, we gathered user input, created an item object, and added it to an array called `items`. We then updated the UI to reflect the changes using the `populateList` function, which generated HTML elements based on the array data.

✅ **Toggling Item State**: We implemented item state toggling by listening for clicks on checkboxes in the `itemsList`. When a checkbox is clicked, the `toggleDone` function is triggered. It checks if the clicked element is an input, updates the item's "done" status in the array, and saves the changes to Local Storage. The UI is then refreshed with the updated data.

By understanding these concepts, we've unlocked the ability to create interactive web applications that can store and display user-generated data. As we continue our 30-day JavaScript journey, we'll explore more fascinating JavaScript concepts and build even more exciting projects! 🌟📋 #JavaScript #LocalStorage #EventListeners #WebDevelopment #30DaysJSChallenge


# Video

<a href="https://youtu.be/WwCCguzIh9k">Click here to see Video</a>