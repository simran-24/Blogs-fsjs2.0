# Play with FlexBox

# FlexBox : -

Flexbox is a property of CSS for making a flexible box, but it is the older version. Nowadays. Flex is used in place of flexbox; we can also use inline flex.

# Flex: -  

Flex is a property of CSS which helps us to make perfect layout of all items in container. By using flex , we can use some properties of flex in CSS to setting up the directions , alignment etc. 

# Properties of Flex : - 

The properties of flex is based on two terms i.e

- Parent 
- Child

## Properties for Parent : - 

In this, the properties of Flex are given in the container and all the items will get affected by the property given in Parent.

Container is the Parent and items are children

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668925963656/W0VatCg9W.png align="left")



### display

 By default, all the items will cover the block area, so it is required to give property display as flex. so that all the items will start work accordingly. Container can be class or id or any tag which is performing the role of parent and contains child in it.

**Syntax :-** 

 
```
body
{
  display:flex;
}
.container 
{
	display:flex;
}

#container
{
	display:flex;
}
``` 

**Before display : flex**

<iframe height="300" style="width: 100%;" scrolling="no" title="display" src="https://codepen.io/simran-24/embed/KKeZNgw?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

**After display : flex**

<iframe height="300" style="width: 100%;" scrolling="no" title="display-flex" src="https://codepen.io/simran-24/embed/BaVJQLb?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>


### flex-direction

Flex-direction is the property which tells the element in which position they need to be get aligned either it's in row or column. 

> flex-direction contains *four *values in it i.e., row, row-reverse, column, column-reverse, By default, it is row.


** Syntax :-**

 
```
container 
{
	display:flex;
    flex-direction: row | row-reverse | column | column-reverse;
}

``` 

-  **row: -**

The elements got aligned in row in starting of the flex from **item 1 **to **item n<sup>th</sup>.**


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668949297863/kzypkNZib.png align="left")

**Syntax :-**

 
```
container 
{
	display:flex;
    flex-direction: row;
}

``` 

**Example :-**

<iframe height="300" style="width: 100%;" scrolling="no" title="row" src="https://codepen.io/simran-24/embed/bGKaRKW?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

-**  row-reverse: -**

The elements got aligned in row in starting of the flex from **item 1 **to **item n<sup>th</sup>.**


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668952853156/MSbcSNZ1L.png align="left")

**Syntax :-**

 ```
container 
{
	display:flex;
    flex-direction: row-reverse;
}
``` 

** Example :-**

<iframe height="300" style="width: 100%;" scrolling="no" title="row-reverse" src="https://codepen.io/simran-24/embed/dyKJzVO?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>

-  **column: -**

The elements got aligned in column in the starting of flex from **item 1 **to **item n<sup>th</sup>.**


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668953465627/BlnRwF8J_.png align="left")

**Syntax :-**
 
```
container 
{
	display:flex;
    flex-direction: column;
}

``` 
 **Example:-**


<iframe height="300" style="width: 100%;" scrolling="no" title="column" src="https://codepen.io/simran-24/embed/zYapdjx?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>

-  **column-reverse: -**

The items got aligned in a column but in reverse order or we can say the alignment will start from the end from **item 1 **to **item n<sup>th</sup>.**


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668953789506/APlvxN0bZ.png align="left")

**Syntax :-**

 
```
container 
{
	display:flex;
    flex-direction: column-reverse;
}

``` 

** Example**

Scroll down to see the result.

<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/gOKoxKv?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>


### flex-wrap


In flex , all the items got aligned in one-line and if we add some items in the flex it also add them in the same by reducing the width of the other items to get the new item adjusted in the same line.But some time we want to add some new items in the new line rather than to add them in the same line 
For that purpose, we will use the flex property *“flex-wrap”*.


> flex-wrap contains three values in it i.e. wrap , nowrap, wrap-reverse, By default, it is nowrap. 



![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668966242279/e1JLLZcM0.png align="left")

> Now, if we add some items or boxes it will reduce the previous one's width and fits in the one line only,either we provide the width explicitly or not.



![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668966702978/zKvdnGPOF.png align="left")


 **Syntax:- **


```
container
{
display : flex ;
flex-wrap : no wrap | wrap |wrap-reverse;
}
``` 

**Example :- 
**
Uncomment the remaining code and see the difference between no wrap and wrap.


<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/GRGyydO?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">

</iframe>


- ** wrap :- **

It will take the another line  if the items excess to get fit in one line. The items got aligned in the row-order only.

> The space between the lines will be according to the container's height only.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668968101106/zbC0ljNLb.png align="left")

**Syntax :- **


```
container
{
  display:flex;
  flex-wrap:wrap;
``` 

**Example :- **

<iframe height="300" style="width: 100%;" scrolling="no" title="wrap" src="https://codepen.io/simran-24/embed/yLEppwm?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

-  **wrap-reverse:- **

It will also take the another line if the items excess to get fit in one line but in reverse order. In simple words, 
the items got aligned in row order but from the bottom of the container 



![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668968806511/FIJ0HdImi.png align="left")

 **Syntax :- **


```
container
{
  display:flex;
  flex-wrap:wrap-reverse;
``` 

** Example :- **

Uncomment the CSS code to see the result of nowrap also.
<iframe height="300" style="width: 100%;" scrolling="no" title="wrap-rev" src="https://codepen.io/simran-24/embed/poKpazM?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>


### justify-content  

justify-content is the property of flex which shuffle up the items of container horizontally.
There are many value are used in justify-content.

> By default, justify-content value is flex-start.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668949297863/kzypkNZib.png align="left")


**Syntax :-**

```
container
{
	justify-content: flex-start | flex-end | center | left | right | start | end | space-around | space-between | space-evenly; 
}

``` 


**-  flex-start **

flex- start works as a direction “row”, it will align the items from the starting of the row.


**Syntax :-**

```
container
{
    display:flex;
	justify-content: flex-start; 
}

``` 


** Example :- **

<iframe height="300" style="width: 100%;" scrolling="no" title="flex-start" src="https://codepen.io/simran-24/embed/zYapeZo?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  </iframe>

- **flex-end**

flex- end will align the items from the end of the row but from item n<sup>th</sup> to item 1.

 **Syntax :-**

```
container
{
     display:flex;
	justify-content: flex-end; 
}

``` 


**Example :- **

Scroll right to see the result.

<iframe height="300" style="width: 100%;" scrolling="no" title="flex-end" src="https://codepen.io/simran-24/embed/zYapezN?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

-** center **

center will align the items in the center of the container.

**Syntax :-**

```
container
{
    display:flex;
	justify-content: center; 
}

``` 

** Example :- **

Scroll right to see the result.

<iframe height="300" style="width: 100%;" scrolling="no" title="center-justify" src="https://codepen.io/simran-24/embed/ExRorrw?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
   </iframe>

-** left or start**

left will align the items in the left side of the container.

> If we give the flex-direction with justify-content, it will start behaving according to the values of flex-direction. we can also use "start" value . It behaves in the same way as left.

**Syntax :-**

```
container
{
    display:flex;
	justify-content: left;  /* start */
}

``` 

**Example :- **

Uncomment the code one by one to see the different result.

<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/KKeZEvq?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>



-** right or end**

right will align the items in the right side of the container.

> If we give the flex-direction with justify-content, it will start behaving according to the values of flex-direction. we can also use "end" value . It behaves in the same way as right.
 
But there is one difference between both ***right*** and *end* that when we give the** *flex-direction*** as ***column or column-reverse*** in ***justify-content :right ***it will stop working means items got aligned according to flex-direction value, but in the ***end ***value the items got aligned from the end of the container.

**Syntax :-**

```
container
{
    display:flex;
	justify-content: right;  /* end */
}

``` 


**Example :- **
<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/rNKpRvK?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>


- **space-around **

space-around will align the items with space around in each item that means each item will contain space from  right and left without specifying them according to the container.

**Syntax :-**

```
container
{
    display:flex;
	justify-content: space-around;
}

``` 

** Example :- **


<iframe height="300" style="width: 100%;" scrolling="no" title="space-around" src="https://codepen.io/simran-24/embed/LYreojO?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>

 **- space-between**

space-between will align the items with space between in each item that means each item will contain space in between two items only.

**Syntax :-**
```
container
{
    display:flex;
	justify-content: space-between;
}

``` 

**Example**

<iframe height="300" style="width: 100%;" scrolling="no" title="space-between" src="https://codepen.io/simran-24/embed/dyKJEee?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>



- **space-evenly **

space-evenly will align all the items with equal amount of space from right and left of the item.

**Syntax :-**

```
container
{
    display:flex;
	justify-content: space-evenly;
}

```

 **Example :- **

<iframe height="300" style="width: 100%;" scrolling="no" title="space-evenly" src="https://codepen.io/simran-24/embed/NWzXVBK?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>  


- ### align

There are two properties for with name *align* in parent properties.
       
- align-items
- align-content



- ### align-items

align-items is working as property ***justify-content*** but the difference is that, align-items will align the items vertically. 

> Some of the values are also same as in justify-content.

 **Syntax :- **


```
container
{
    display:flex;
	align-items: flex-start | flex-end | center | stretch;
}
``` 

- **flex-start**  

The items aligned at the starting of the flex container.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669039456628/ay3nI7zjD.png align="left")


- **flex-end**
The items aligned at the starting of the flex container (vertically).


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669039824931/P8Ty42fCq.png align="left")


- **center**

The items aligned in the middle of the flex container (vertically).

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669039942448/ACIq9qDeM.png align="left")


- **stretch**

stretch will work until we give height of the item.

**Before giving height :-**

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669040579122/r2OWsl_WK.png align="left")

**After giving height :-**`According to height given in *height* property.
 
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668949297863/kzypkNZib.png align="left")

**Example :- **

<iframe height="300" style="width: 100%;" scrolling="no" title="align-items" src="https://codepen.io/simran-24/embed/eYKVOpN?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

- ### align-content

align-content will align the lines vertically(the whole line of the container), it will work on multiple lines.
So,it is necessary to use multiple lines to see the result of ***align-content***. 

> To use multiple line, we need to use "flex-wrap : wrap or wrap-reverse" . because "nowrap" will give no effect to result.

 **Syntax :- **


```
container
{
    display:flex;
	align-content: flex-start | flex-end | center | stretch | space-around | space-between ;
    flex-wrap: wrap ;   /* wrap-reverse */
}
```

- **flex-start**  

The items aligned at the starting of the flex container.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669049956297/KFzUbQK8t.png align="left")


- **flex-end**
The items aligned at the end of the flex container (vertically).

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669050175999/WX2YikQ5s.png align="left")

- **center**

The items aligned in the middle of the flex container (vertically).

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669050615935/qaOaSDuxP.png align="left")

- **space-around**

space-around will align the items with space around in each line that means each line will contain space from top and bottom without specifying them according to the container.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669051179942/vgSXmlGqB.png align="left")

- **space-between**

space-between will align the items with space between in each line that means each line will contain space in between two lines only.



![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669051719777/vCUhcz2ae.png align="left")

- **stretch**

stretch will work until we give height of the item.

**Before giving height :-**

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669052170659/g7vdkBuTQ.png align="left")

**After giving height :-**`According to height given in *height* property.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669049956297/KFzUbQK8t.png align="left")

**Example :- **
Uncomment the code one by one to see the result.

<iframe height="300" style="width: 100%;" scrolling="no" title="align-content" src="https://codepen.io/simran-24/embed/bGKLVEV?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>


## Properties for Child: -

In this, the properties of Flex are given in the child and that particular the items will get affected by the property given instead of all the items.

### Syntax 


```
container
{
    display:flex
}
item
{
    properties : value;
}
``` 


- ### order 

 order property will work on the order of alignment of items. In simple words, we can say that initial order of 
all the items is 0 and can be increased by infinite value according to the items. By using order property, we can change the order of each item as per our requirements.

It works as mostly as a graph.

> Suppose we have only 10 items and how we can give order 100 to any item. But it will work as that particular item having order 100 will be shifted at the end. This is how it works.

**For main Axis(Horizontal) : - **


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669112072406/QGAw8YTcT.png align="left")

**For cross Axis(Vertical) :- **


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669112420244/vcN7vpdh8.png align="left")



> ** Note :- The initial order for all the items will be zero & Only the items with order will change their order other items will remain at the same order value i.e 0. but will change the position.
**


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669114559201/ZG3KPSf72.png align="left")


Now, if we change the order of item2 as 1 and item1 as 2 . It will come like the below image.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669114803289/5yw1AVTiZ.png align="left")

or, if we give the order of item2 as -2 and item1 as -1. The result will be :- 


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669115017450/ZPvGjA9qE.png align="left")

**Syntax :- **


```
container 
{
  display:flex;
}
item
{
  order: 0 | 1 | 2 |........| infinite; /*negative values are allowed */ 
}
``` 


**Example :- **

<iframe height="300" style="width: 100%;" scrolling="no" title="order-flex" src="https://codepen.io/simran-24/embed/bGKLLvJ?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>


- ### flex-grow 
       flex-grow will increase the size of particular item by number of times. Initial value of flex-grow is 1.

> If we give flex-grow :2, the size of that item will increase two times of the other item and value goes upto infinite but according to the items present. 

With value 1,2,3 and 4 
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669118667643/Z5ZqRkoZ0.png align="left")

With value 1,6,7 and 8

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669118735328/Pi_9svG9U.png align="left").

> it will adjust the width of all the items according to the width of the container.

**Syntax **


```
container 
{
  display:flex;
}
item
{
     flex-basis: value; /* as we set in width or height */
    flex-grow:1 | 2| 3 ......| infinite ; /* negative values are invalid*/
}
``` 

** Example :- **

<iframe height="300" style="width: 100%;" scrolling="no" title="grow-flex" src="https://codepen.io/simran-24/embed/qBKxoGw?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  </iframe>
   
- ### flex-shrink
flex-shrink will decreases the size of items. The initial value of flex-shrink is 1.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669126882690/5qeweQTUm.png align="left")

> We need to set the width of flex-basis of all the items to see the result of flex-shrink. flex-basis is the property to set the width of the items for flex-grow and flex-shrink.

**Syntax :- **


```
container 
{
  display:flex;
}
item
{
    flex-basis: value; /* as we set in width or height */
    flex-grow:1 | 2| 3 ......| infinite ; /* negative values are invalid*/

``` 

**Example :-**

<iframe height="300" style="width: 100%;" scrolling="no" title="shrink" src="https://codepen.io/simran-24/embed/Yzvejdm?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

- ### align-self

This property will align the specified items in vertical manner (on cross-axis).It works as align-items but the difference is that it will align the particular item instead of all items.

It has mainly five values : 

 **Syntax :- **


```
container
{
    display:flex;   
}
item
{
	align-content: auto | flex-start | flex-end | center | stretch  ;
}
```
- **auto**  
It is the default value . No effect will be there.
 
**Syntax :- **

```
container
{
    display:flex;   
}
item
{
	align-self: auto ;
}
```

- **flex-start**  

The item will aligned at the starting of the flex container (at the top).
**Syntax :- **

```
container
{
    display:flex;   
}
item
{
	align-self: flex-start ;
}
```

- **flex-end**
The items aligned at the end of the flex container (at the end).

**Syntax :- **

```
container
{
    display:flex;   
}
item
{
	align-self: flex-end ;
}
```

- **center**

The items aligned in the middle of the flex container (between top and bottom).
**Syntax :- **

```
container
{
    display:flex;   
}
item
{
	align-self: center ;
}
```
- **stretch**

stretch will work until we give height of the item.

**Syntax :- **

```
container
{
    display:flex;   
}
item
{
	align-self: center ;
}
```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1669129678314/jBjadHzdR.png align="left")

**Example :- **

<iframe height="300" style="width: 100%;" scrolling="no" title="align-content" src="https://codepen.io/simran-24/embed/rNKJZzP?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

## Shorthand Properties :- 


- flex-flow : -  It is the shorthand property of ***flex*** and *flex-direction*.
  
Syntax :- 
   
```
item 
{
flex-flow : column wrap | row wrap ;
}
``` 


- flex:-  It is the shorthand property of ***flex-grow or shrink*** and *flex-basis*.

Syntax :- 
   
```
item
{
flex :  <flex-grow || shrink> | flex-basis ;
}
``` 
# Summary 

In this article, we have covered flex basics and its properties. We also covered the shorthand properties of flex which is mostly used. 

**Source Code Link :-** 

https://github.com/simran-24/19Nov-fsjs-2.0/tree/main

Hope it was helpful!

Happy Learning!!

See you soon......


![tenor.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1669130372358/9rMb_7CQE.gif align="left")



