**Day 13: Adding Smooth Image Slide-In Effects with JavaScript**

On Day 13 of our 30 Days JavaScript Challenge, I dove into the world of event listeners and functions to create a delightful image slide-in effect. Here's the essence of what I learned:

📸 **Selecting Slide-In Images**: We began by selecting all elements with the class "slide-in" using `document.querySelectorAll`. These are the images we want to slide into view as the user scrolls.

🚀 **Creating the Magic**: The `checkSlide` function was the star of the show. Inside it, we iterated through all the selected `sliderImages`. For each image, we calculated two key values:

1. `slideInAt`: This represents the point where the image should start sliding in. It's calculated as the current vertical scroll position (`window.scrollY`) plus half the height of the viewport (`window.innerHeight`) minus half the height of the image itself (`sliderImage.height / 2`).

2. `imageBottom`: This indicates the bottom position of the image, calculated as the sum of the image's top offset (`sliderImage.offsetTop`) and its height.

We then checked two conditions:

- `isHalfShown`: We determined if the image is at least halfway into the viewport by comparing `slideInAt` with the image's top offset.

- `isNotScrolledPast`: We ensured that the image is not scrolled past by comparing the current scroll position (`window.scrollY`) with the `imageBottom`.

🌟 **Adding the Magic Class**: When both conditions were met, indicating that the image should be visible in the viewport, we added the "active" class to the image using `sliderImage.classList.add('active')`. This class likely contains CSS rules to transition the image into view smoothly.

🔮 **Debouncing Scroll Events**: To optimize performance and prevent excessive function calls during scrolling, we attached the `checkSlide` function to the "scroll" event using `window.addEventListener`. But, to ensure it doesn't execute too frequently, we wrapped it in a `debounce` function.

This enchanting code creates a captivating user experience by smoothly sliding images into view as the user scrolls down the page. As our 30-day JavaScript journey continues, we'll keep exploring exciting JavaScript concepts and techniques. Stay tuned for more captivating discoveries! 🌈🖼️ 

# video

<a href="https://youtu.be/54NmQjAXJ_0">Click here to see video</a>