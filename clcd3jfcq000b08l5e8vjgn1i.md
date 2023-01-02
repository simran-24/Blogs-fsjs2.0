# Level Up with Positions in CSS

Before starting with the position in CSS. We need to know the basic meaning of the position.

# Position

In general, Positions have more than one meaning which means they can be a status, place and conditions and many more.

In CSS, position means locality of items, or we can say that it is the place where the items reside. It is the property of CSS which has some values.

> After giving the property *position*, we will be able to give other properties of CSS as top, right, bottom and left.

## Values or Types of Position

There are 5 values of position: -

* static
    
* relative
    
* absolute
    
* fixed
    
* sticky
    

## static

static is ***by default*** the value of the position property. The item got placed according to the normal flow of the layout.

### **Syntax**

```css
item
{
    position:  static;
}
```

> Nothing will be shown after giving the static property. All the items are in the normal flow of the page layout.

### **Example**

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1670351700293/fmOfhjp6l.png align="left")

## relative

the ***relative*** will also work on the normal flow of the page layout but after giving extra properties like the top, right, bottom and left. it will get affected and will start shifting from its original position.

### **Syntax**

```css
item
{
    position:  relative;
    top : 10px ;
  /* right : 10px;
    bottom:10px;
    left:10px; */
}
```

### **Example**

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1670352324330/KAVLlA90h.png align="left")

> The original position of Box 2 is where it currently resides and after giving top, right, bottom or left properties it will start shifting from its X-axis and y-axis which is highlighted in a circle.

## absolute

absolute will be taken out from the normal flow of the layout; it will be treated by other items as if it does not exist. The position of the absolute will be near its parent block.

### **Syntax**

```css
item
{
    position:  absolute;
    top : 10px ;
  /* right : 10px;
    bottom:10px;
    left:10px; */
}
```

### Example

![Box1.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1670352759976/-yoz-ndDR.gif align="left")

## fixed

The fixed position will make the element fixed on the page regardless of scrolling up, down, left or right; the element will stay at its position i.e., fixed.

### **Syntax**

```css
item
{
    position:  fixed;
  
}
```

### **Example**

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1670353194313/eePzWOpfi.png align="left")

After scrolling down all the other boxes got disappeared but the box with fixed property is still showing.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1670353214901/nij1hnL7E.png align="left")

## sticky

sticky will work something the same as the position fixed when it reaches its threshold value. Before reaching the threshold value, it will work as a relative.

> sticky is also known as a Hybrid of relative and fixed.

### **Syntax**

```css
item
{
    position:  sticky;
    top:10px; /*threshold value*/  
}
```

### **Example**

%[https://youtu.be/FiYdZFw5n5I] 

# Summary

In this article, we learned about the position properties of CSS. We have seen that all properties have their own usage, syntax and Examples.

Source Code :- [19-Nov-Fsjs2.0/Position\_Sticky at main · simran-24/19-Nov-Fsjs2.0 (](https://github.com/simran-24/19-Nov-Fsjs2.0/tree/main/Position_Sticky)[github.com](http://github.com)[)](https://github.com/simran-24/19-Nov-Fsjs2.0/tree/main/Position_Sticky)

Hope it was helpful!

HAppy LearNing :)

![See the source image](https://media1.tenor.com/images/88ae11548eb77b751325c3ff493cddcc/tenor.gif?itemid=11819904 align="left")