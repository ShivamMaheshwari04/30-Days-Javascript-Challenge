# Day - 6

Creating an Ajax Type Ahead for City and State Search

Today was an exciting day in my coding journey. I embarked on a project to create an Ajax Type Ahead application that allows users to search for city and state names, receiving real-time suggestions as they type. This project was a significant learning experience, as it introduced me to various concepts and technologies, including regex, API requests, fetch, mapping data, filtering, event listeners, and much more.

By the end of the day, I had a fully functional Ajax Type Ahead application that allowed users to search for city and state names with ease. This project not only expanded my technical skills but also taught me about the importance of user experience and error handling in web development. I'm excited to continue building on this project and explore more advanced concepts in the days to come

# Video 

<a href="https://youtu.be/gEpCizxMhQc"> Click here to see video of my project </a>

<hr>

# About Regex (Regular Expression)

Regex, yaani (Regular Expression), ek special sequence of characters hai jo text pattern ko represent karta hai. Yeh ek programming concept hai aur ek string pattern ko define karne ke liye use hota hai. Aap is pattern ko string ke andar search, match, replace, aur manipulate karne ke liye istemal karte hain.

Yeh ek aisa powerful tool hai jo text data ko search aur manipulate karne mein madad karta hai. Ye patterns (patterns) ko define karne mein use hota hai, jaise ki specific strings, characters, ya formats. Isse aap text mein complex search aur replace operations perform kar sakte hain.Chaliye ek simple example dekar samjhte hain: 


Maan lo, aapko ek document mein phone numbers dhoondne hain jo 10 digits ke hain, aur woh kisi bhi form mein ho sakte hain, jaise ki "1234567890" ya "(123) 456-7890".Yahan regex ka use karke aap yeh kaam kar sakte hain:

**Code**
<pre>
<b>
// Regex pattern for 10-digit phone numbers 
**var regex = /\d{10}/g;**

// Text to search for phone numbers 
**var text = "Mere contacts mein kuch numbers hain: 1234567890, (987) 654-3210, aur 555-12345.";**

// Use regex to find all phone numbers in the text
**var matches = text.match(regex);**

// Print the matches
**console.log(matches);**
</b>
</pre>
Is example mein, /\d{10}/g ek regex pattern hai jo 10 digits ko match karega. Yeh pattern \d se start hota hai jo ek digit ko represent karta hai, aur {10} specifies ki exactly 10 digits ko match karna hai. g flag global search ko indicate karta hai, jisse ki sabhi matching numbers milenge.

Jab aap is code ko run karenge, to output mein aapko 1234567890 aur 5551234567 milenge, jo ki 10-digit numbers hain.

Regex ek versatile tool hai aur aap iska istemal text processing, data validation, aur bahut se aur use cases mein kar sakte hain

<hr>

# Fetch Function 

Fetch ek JavaScript function hai jo web requests ko bhejne aur server se data ko retrieve karne ke liye istemal hota hai. Fetch function modern web applications mein data fetch karne ke liye bahut hi powerful aur flexible tool hai. Yeh ek Promise-based API hai, iska matlab hai ki aap async/await ya Promise chaining ke sath fetch requests ko manage kar sakte hain.

<b> Fetch function ka basic syntax is tarah hota hai:
<pre>
fetch(url, options)
  .then(response => {
    // Handle the response
  })
  .catch(error => {
    // Handle errors
  });
</pre>

</b>

Yahan, url parameter ek string hota hai jo aapke request ke endpoint ya URL ko represent karta hai. options parameter ek optional object hota hai jo aapke request ko customize karne ke liye istemal hota hai, jaise ki request method, headers, aur body.

Fetch function ek Promise return karta hai, isliye aap .then() aur .catch() methods ka istemal karke response ko handle kar sakte hain.

**Ek example dekhte hain jahan hum JSON data fetch karte hain:**
<pre>
<b>


fetch('https://api.example.com/data')
  .then(response => {
    if (!response.ok) {
      throw new Error('Network response was not ok');
    }
    return response.json(); // Parse response as JSON
  })
  .then(data => {
    console.log(data); // Process the JSON data
  })
  .catch(error => {
    console.error('There was a problem with the fetch operation:', error);
  });

</b>  
</pre>

Is example mein, hum ek GET request bhejte hain https://api.example.com/data URL par, phir response ko check karte hain ki kya woh sahi aaya hai (response.ok). Agar response theek nahi hai, to hum ek error throw karte hain. Agar response sahi hai, to hum JSON data ko parse karte hain aur us data ko console par print karte hain.

Fetch function aapko data fetch karne aur server ke saath communication karne mein madad karta hai, aur aap ise various HTTP methods (GET, POST, PUT, DELETE, etc.) ke sath istemal kar sakte hain. Isse aap web applications mein data ko dynamic tarike se load aur update kar sakte hain.
