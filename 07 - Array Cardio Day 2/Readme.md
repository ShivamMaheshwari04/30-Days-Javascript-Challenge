# Day - 7
On Day 7 I Learn about array function i manipulate array with these function and get useful information in a few lines of code.In this project i learn some,every,splice,find,findIndex,Arrow Function.


# Array Function in JS 

Sure, here's an explanation of those JavaScript array methods in Hinglish with examples:

1. `Some` : Ye function array ke har ek element par check karta hai, aur agar kisi ek element mein condition sahi ho jati hai toh true return karta hai, warna false.

   Example :
   ```javascript
   const numbers = [1, 2, 3, 4, 5];
   const isEven = (num) => num % 2 === 0;
   const hasEvenNumber = numbers.some(isEven);
   console.log(hasEvenNumber); // true (kyunki 2 even hai)
   ```

2. `Every` : Ye function array ke har ek element par check karta hai, aur tab true return karta hai jab saare elements condition ko satisfy karte hain, otherwise false.

   Example :
   ```javascript
   const numbers = [2, 4, 6, 8, 10];
   const isEven = (num) => num % 2 === 0;
   const allEven = numbers.every(isEven);
   console.log(allEven); // true (kyunki sab even hain)
   ```

3. `Splice` : Ye method array mein changes karta hai, kisi specific index se elements ko add, remove, ya replace karne ke liye use hota hai.

   Example :
   ```javascript
   const fruits = ['apple', 'banana', 'cherry', 'date'];
   fruits.splice(1, 2, 'grape', 'fig'); // Removes 'banana' and 'cherry', adds 'grape' and 'fig' at index 1
   console.log(fruits); // ['apple', 'grape', 'fig', 'date']
   ```

4. `Find` : Ye function array mein ek specific condition ko satisfy karne wala pehla element deta hai. Agar koi element condition ko satisfy nahi karta, toh undefined return hota hai.

   Example :
   ```javascript
   const numbers = [10, 20, 30, 40, 50];
   const findNum = numbers.find((num) => num > 25);
   console.log(findNum); // 30 (kyunki 30 pehla number hai jo 25 se bada hai)
   ```

5. `FindIndex` : Ye function array mein ek specific condition ko satisfy karne wala pehla element ka index deta hai. Agar koi element condition ko satisfy nahi karta, toh -1 return hota hai.

   Example :
   ```javascript
   const numbers = [10, 20, 30, 40, 50];
   const findIndexNum = numbers.findIndex((num) => num > 25);
   console.log(findIndexNum); // 2 (kyunki 30 index 2 par hai aur 25 se bada hai)
   ```
   
