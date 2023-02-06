# Walk through the JavaScript Array

### Let's understand the basic meaning of an array.

# Array

An array is a type of data structure that contains different items with different datatypes. All the items in the array are stored at contiguous memory locations.It uses indexing which means each item has some index value with it.

> The index value starts from 0 in the array.

## Syntax

```javascript
let arrayname=[item1,item2,......,so on];
console.log(arrayname);
```

> "let" is a keyword in javascript that is used to declare the variable.

## Example

```javascript
let arr=[1,2,3,"Alpha",3.5,true];
console.log(arr);
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1671354898667/jnvg_bbPO.png align="center")

> In this example, An array contains items with different data types i.e. numeric, string, bool and decimal.

# Array Methods

An array in JavaScript has a lot of methods but here we will explain the bare minimum of them.

### (i) concat() :-

***<mark>concat</mark>*** word comes from the word "<mark>concatenate</mark>" which means to merge two or more items and make them one without making any changes in the original array.

### Syntax

```javascript
let array1 = [item1,item2,item3,item4,....so on];
let array2 = [item5,item6,item7,.....so on];
console.log(array1.concat(array2));

// Or concatenate more than 2 arrays

let array1 = [item1,item2,item3,item4,....so on];
let array2 = [item5,item6,item7,.....so on];
let array3 = [item8,item9,item10,....so on];
console.log(array1.concat(array2,array3 ,.....,arrayN));
```

> we can concatenate two or more two arrays within one array.

### Example 1

Concatenate two arrays.

```javascript
let arr=["C","C++","Java"];
let arr2=["JavaScript","HTML","CSS"];
console.log(arr);
console.log(arr2)
console.log(arr.concat(arr2));
```

Output:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672592612970/46009045-b029-4703-8b49-ed38c0b9a9b8.png align="center")

### Example 2

Concatenate more than two arrays.

```javascript
let arr=["C","C++","Java"];
let arr2=["JavaScript","HTML","CSS"];
let arr3=["ReactJS","NodeJS"];
console.log(arr);
console.log(arr2)
console.log(arr3);
console.log(arr.concat(arr2,arr3));
```

Output:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672592821311/e6fb7f8c-30fe-49c5-aa62-b31e09993759.png align="center")

### (ii) toString() :-

It is an array method that is used to convert the array items into a string and it will separate the array items by comma (,).

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....so on];
console.log(array_name.toString());
```

### Example

```javascript
let arr=["C","C++","Java","JavaScript","HTML","CSS"];
console.log(arr);    //[elements in square brackets are array]
console.log(arr.toString()); //element without square brackets are string
```

Output:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672593294717/b703ebe3-869f-472b-98db-0ffebd700196.png align="center")

> **Note:**\- We can check the type of element by using the ***typeof()*** method.
> 
> <mark>But remember, it is not an array method.</mark>
> 
> **typeof():-**
> 
> typeof() method will take the variable name as a parameter and give the type of that variable as an output or result.
> 
> **Syntax**
> 
> ```javascript
> let variable_name = value;
> console.log(typeof(variable_name));
> ```
> 
> **Example**
> 
> ```javascript
> let arr=[1,2,3,4,5];
> console.log(arr);
> console.log(typeof(arr))
> let str=arr.toString();
> console.log(str);
> console.log(typeof(str));
> ```
> 
> Output :-
> 
> ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672594311133/1d021285-e46a-4256-be8f-e4c8d8d11193.png align="center")

### (iii) join() :-

join() is also an array method that converts an array into a string same as in the **toString()** method.

> But additionally, we can specify the separator of our choice.

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....so on];
console.log(arr.join());       //
console.log(arr.join(" "));   //seprate with whitespace
console.log(arr.join("Seprator")); //Seprator Symbol will show between each element
```

### Example

```javascript
let arr=["C","C++","Java","JavaScript","HTML","CSS"];
console.log(arr);
console.log(arr.join());
console.log(arr.join(" "));
console.log(arr.join("*"));
```

Output:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672595523534/991e488c-b5b3-43cb-affb-c3fb7934b6e2.png align="center")

### (iv) pop() :-

The pop() method will remove the element from the ***last index*** of an array.

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....,itemN];
console.log(array_name.pop());
```

### Example

```javascript
let arr=["C","C++","Java","JavaScript","HTML","CSS"];
let popvar=arr.pop();
console.log("The item that has been deleted is : " + popvar);
console.log("Array after deletion : " + arr);
```

Output:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672596135259/faf80370-a4a8-4122-bc2e-376f8e9a4135.png align="center")

### (v) push() :-

push() method is used to add an element to an array. It will push the element to the ***last index*** of the array.

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....,itemN];
console.log(array_name.push("element")); //element is a value to be added in an array list
```

### Example

```javascript
let arr=["C","C++","Java","JavaScript","HTML","CSS"];
let pushvar=arr.push("Tailwind CSS");  //pushvar variable return the new length of the array
console.log("The Length of an array element after addition is : " + pushvar);
console.log("Array List after adding an element : " + arr);
```

Output:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672596914909/2db1de0e-3a8e-4132-a445-2b64adf5aaa1.png align="center")

> Now, What if we want to add or remove the element from the starting index ???
> 
> The answer is "There are some methods to do so."; i.e. ***shift() and unshift()***.

### (vi) shift() :-

shift() method is used to delete the element from the ***starting or first index*** of an array.

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....,itemN];
array_name.shift();  //delete the first item i.e. item1
console.log(array_name);
```

### Example

```javascript
let arr=["C","C++","Java","JavaScript","HTML","CSS"];
let shiftvar = arr.shift();
console.log("The item that has been deleted is : " + shiftvar);
console.log("Array after deletion : " + arr);
```

Output: -

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672597960763/23839ba4-d0a0-4c47-988e-4043c6c5ae64.png align="center")

### (vii) unshift() :-

unshift() method is used to add the element from the ***starting or first index*** of an array.

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....,itemN];
array_name.unshift(element);  //add the item at first index 
console.log(array_name);
```

### Example

```javascript
let arr=["C","C++","Java","JavaScript","HTML","CSS"];
let unshiftvar = arr.unshift("ReactJS");
console.log("Array Length after adding one element : " + unshiftvar);
let unshiftvar2=arr.unshift("NodeJS");
console.log("Array Length after adding second element : " + unshiftvar2);
console.log("Array list after adding elements : " + arr);
```

Output:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672599260529/1dcbca34-6feb-49dc-82ee-1ede24a7fc12.png align="center")

### (viii) at() :-

at() is a method that will take an integer it doesn’t get affected whether it’s a positive integer or negative integer. An integer will be the index number. It will access the element of the given index from the array.

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....,itemN];
console.log(array_name.at(index_value));      //returns the value present at that index
```

### Example

```javascript
let arr=["C","C++","Java","JavaScript","HTML","CSS"];
console.log(arr.at(2));          
console.log(arr.at(-2));
//length of array is 6 but below index number is greater than the array length
console.log(arr.at(10));   // results undefined
```

> NOTE:- if the index value is more than the array length then, the result will be ***<mark>undefined</mark>.***

Output:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672600577896/b53a8953-49f0-4549-92ae-fb1c5aa8eabd.png align="center")

> We can also access the array element and change its value by using an index number.

```javascript
let arr=["C","C++","CSS","Java","JavaScript","HTML"];
console.log("Before changing the value is " + arr[2])
arr[2]="TailwindCSS";
console.log("After changing the value is : " + arr[2]);
```

Output:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672600830889/867b66dc-4b1a-4aef-80dc-913b8bcf60ef.png align="center")

### (ix) copyWithin() :-

copyWithin() is a method that is used to copy array elements at a different location in the same array within a given range.

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....,itemN];
array_name.copyWithin(target_values,start-value,end-value);

// Or 
array_name.copyWithin(target_values);  //start and end is optional
```

### Example

```javascript
let arr=["C","C++","Java","JavaScript","HTML","CSS"];
arr.copyWithin(5);    //by default, first element get copied at target
console.log(arr);
arr.copyWithin(1,3,5) ; //change the element at first index with element present at index 3 till 5 i.e. 
console.log(arr);
```

> Note: - ***end*** value should not be less than the start value otherwise it will copy nothing for the end value.

Output:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672642407419/dade5cf3-d44b-45af-9b37-c6f174d391ec.png align="center")

> Note: - Original array will get modified after implementing <mark>copyWithin()</mark> method.

### (x) fill() :-

fill() is a method that is used to change the value of an element in an array at a specified index or in a range. It works somewhat like copywithin() method. But the difference is, here we provide the value explicitly to get copied in the array.

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....,itemN];
console.log(array_name.fill(value,start_index,end_index)); //change the values at start-index till end-index.
or
console.log(array_name.fill(value)) //change all the values in the array list.

or
console.log(array_name.fill(value,start_index); //change the value from start index till the end of an array.
```

### Example

```javascript
let arr=["C","C++","Java","JavaScript","HTML","CSS"];
console.log(arr.fill("Tailwind"));
console.log(arr.fill("ReactJs",1,3));  
console.log(arr.fill("NodeJS",2));
```

Output: -

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672645356713/d66cacab-f58d-4212-a95f-de3915c4a6e5.png align="center")

> Note: - Original array will get modified after implementing the <mark>fill() </mark> method.

### (xi) reverse() :-

reverse() is a method that reverses the whole array which means the <mark>last element</mark> of an array becomes the <mark>first element,</mark> the <mark>second last element</mark> becomes the <mark>second element </mark> of an array and so on.

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....,itemN];
console.log(array_name.reverse()); 
```

### Example

```javascript
let arr=["C","C++","Java","JavaScript","HTML","CSS"];
console.log("Original array before reverse is : " + arr);
console.log(arr.reverse());
console.log("Original array after reverse is : " + arr);
```

Output: -

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672646387757/b46d15ff-4149-4e29-814a-7befbe79f787.png align="center")

> Note: - Original array will get modified after implementing the <mark>reverse() </mark> method.

### (xii) slice() :-

slice() method is used to extract the element from the original array and make a copy of that extracted element into a new array. It will not change the original array.

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....,itemN];
console.log(array_name.slice());
// or
console.log(array_name.slice(start,end)); //end value is excluded
```

### Example

```javascript
let arr=["C","C++","Java","JavaScript","HTML","CSS","TailwindCSS","ReactJS"];
console.log(arr.slice());
console.log(arr.slice(3));
console.log(arr.slice(3,5));
console.log(arr.slice(4,-1));
```

Output: -

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672658383403/5c869f82-24d0-43a4-be20-c6363076e86b.png align="center")

### (xiii) splice() :-

splice() method can add new elements to the array or can replace the existing new ones.

### Syntax

```javascript
let array_name = [item1,item2,item3,item4,....,itemN];
console.log(array_name.splice(start_value));

//or
console.log(array_name.splice(start_value,delete_count));
//or
console.log(array_name.splice(start_value,delete_count,new_value));
```

### Example

```javascript
let arr=["C","C++","Java","HTML","CSS","TailwindCSS","ReactJS"];
console.log(arr.splice(5));    //start value
//it will start extracting from index 5 until end of an array
console.log("Array List after giving the start value : " + arr);

console.log(arr.slice(3,5));   //start and delete count
//it will start extracting from index 3 until index 5 i.e 2 elements
console.log("Array List after giving the start value and deletecount : " + arr);

// In below example 0 items will get deleted 
console.log(arr.splice(1,0,"JavaScript")); //start,delete and new value
//it will add new element at index 1
console.log("Array List after giving the start value, deletecount and new value : " + arr);

//// In below example 4 items will get deleted
console.log(arr.splice(1,4,"JavaScript")); //start,delete and new value
//it will delete 4 elements from index 1 till index 4 then will add new element at index 1 
console.log("Array List after giving the start value, deletecount and new value : " + arr);
```

Output: -

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672659305647/bea52fcf-1287-4878-8203-87bfaeb55b23.png align="center")

> In the above example, **arr.splice()** will return the extracted elements from the array.
> 
> **start** means the starting index value from where the element starts getting extracted.
> 
> **Delete** count means how many items should get deleted from the array.
> 
> **End** means until where the method will get implemented.

# Summary

In this article, we learned about the basic methods of an array in JavaScript. we have gone through the syntax and examples of all these methods. I also mentioned some important notes that need to remember while implementing these methods. These are not the only methods of an array there are some more methods present. I will try to cover those methods in the future.

Hope it was Helpful!

HaPPy LeArning! :)

![See the source image](https://media.tenor.com/images/e955f55bab6839ec724531e3bae3303c/tenor.gif align="left")
