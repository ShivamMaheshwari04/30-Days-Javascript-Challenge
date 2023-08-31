# On Day 4

In Day 4, I gain knowledge about arrays through the use of array methods and performing array functions on arrays to get useful information. When I use the array function in some places, I get stuck. Wes Bros. His tutorials help me get rid of errors and explain everything in detail. In this project, I learn about array functions like map,reduce,sort,split, filter, and many more. They give a whole tutorial about how to play with arrays and get as much useful information as you want.

# Defining an array 
let arr = new Array(5);

# Array Methods in Javascript

**Array Insert Functions**

**Push:-** They add an element to an array at the end.
**unshift :-** They add an element to an array in the beginning.
**Splice :-** If you want to insert an element (or elements) into a particular point somewhere within the array, besides the beginning or end, then you should most likely be using the splice() method.

or 
Agar Koi Element Beech Se Delete ya Add Krna Hai Toh aap Spile Ka User Kr Sakte hai


**Syntax =** list.splice(1, 0, "baz"); // at index position 1, remove 0 elements, then add "baz" to that position.

**Example :-** 

let insert  =  {1,2,3,4}
insert.push(9) 
insert.unshift(5);
insert.splice(2,1,5);

<hr>


**Deleting an Element in an Array**

**Pop :-** Removing the End Element
**shift :-** Removing the beginning element
**plice :-** an element from the middle


**Example :-** 

let insert  =  {1,2,3,4}
insert.pop(4) 
insert.shift(1);
insert.splice(1,1); // at index position 1, remove 1 element


<hr>


**Empty an array**

number.length = 0;

<hr>

**Combining and slicing an array** 
// Combining
let first = [1,2,3]
let second = [4,5,6]
let combined = first.concat(second) // arrayName.contact(another array name that you want to concate)




// slicing 


let combined = [1,2,3,4,5,6,7]
let slice = combined.slice(2,4); // arrayName.slice(indexNo.of Starting Index, Excluding Index)


<hr>


**Spread Operator (...)**

This operator is used to combine a array 
let first = [1,2,3];
let second = [4,5,6];
let combined = [...first,0, ...second]; // Output [1, 2, 3, 0 , 4, 5, 6]


<hr>

**Joining an Array**


let number = [10,20,30,40]
const joined = number.join(',') // Output : - 10,20,30,40


**Split a Array**


let message = "This is Message";
let parts = message.split(' ');
console.log(parts) // Output :  [ 'This', 'is', 'Message' ]


<hr>


**Sorting an Array**

Let numbers = [4,5,6,7,1,2,3,4];
numbers.sort();
console.log(numbers)




**Filtering Arrays**


let numbers = [-1,-2,4,5];
let filtered = numbers.filter(function (value){
return value>=0;
});


**Mapping Arrays** :- Maps each element of an array to something else.


let numbers = [-1,-2,4,5];
let filtered = numbers.filter(value => value >= 0);
let map = filtered.map(function (num){
return {value : num};
})

**Reduce** 

**total :-**	Required.
--The initialValue, or the previously returned value of the function.

**currentValue :-**	Required.
--The value of the current element.

**currentIndex :-**	Optional.
--The index of the current element.

**arr :-**	Optional.
--The array the current element belongs to.

**initialValue :-**	Optional.
--A value to be passed to the function as the initial value.

**Youtube Videos Link for Reduce :-**
<a href ="https://www.youtube.com/watch?v=b9zgRt4p9Zo">First Video</a> 
<a href = "https://youtu.be/60eFraqGEv4?si=JeNWJ7M46FWbLtsK">Second Video</a>

<hr>