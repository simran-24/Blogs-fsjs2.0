# Magical CSS....

# CSS

  CSS stands for “Cascading style sheet”. It is used to style the webpage or the whole website.
  As like, we use HTML for structuring the Webpage.

### Let’s take an example: - 
Suppose you wants to build a house , You’ll need an architect to design the whole structure of your house.
Then as per the design the architect will give commands to its labor to structuring the building. 

That’s what the HTML does. As per user ‘requirements, Web designer will make a design of the structure of the website and by using HTML, he/she will make the structure of the web page

Like this:  Before CSS -  ![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668319408475/u2MxcBJdn.png align="left")

But it does not look good enough.

So what will be the next step ??


The answer is that the owner will hire some interior and exterior designers to work on its decoration.
That’s what, CSS will do on the webpages.

Yes, it is used for styling purpose. 

And after applying CSS , the structure of the website will look like this: -

After CSS 
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668319593308/B7ovLu4ol.png align="left")


So now, basic concept is clear that why we use CSS while developing a site.


> What Next ???? 

### Methods of using CSS in HTML document.

How many ways are there to use CSS?

There are mainly three ways to use CSS.

•	Inline

•	Internal

•	External


### Inline CSS
-  Inline CSS :- It is a method in which the stylings are given inside the elements.

For example :- 


```  
 <p style= "background-color : #c6eaa3;">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Magnam sapiente sit perferendis cupiditate! Reprehenderit sequi non dicta eveniet earum ex fugit? Quam doloribus vel quod odio exercitationem quia temporibus sed tempore iure. Aliquid totam sequi, eveniet soluta nemo doloribus. Quod, laboriosam in. Fuga quasi dolorum ipsam quod quo eveniet, mollitia voluptate quas impedit maiores saepe molestiae optio aperiam reprehenderit exercitationem sequi sapiente? Temporibus laboriosam excepturi, </p>
``` 


> But it is not a good way coding, it makes your document look so complex and even no professional can read that source code easily.


### Internal CSS
- Internal CSS :- It is a method to style the webpages by giving the &lt;style&gt; tag inside of head in HTML file.

For example :- 


``` 
<style>
     h1{
        color:#690eea;
     }
     p{
        text-align: justify;
        color: rgb(243, 153, 9);
     }
   </style>
</head>
<body>
    <section>
        <h1>
            Internal CSS
        </h1>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tenetur id architecto omnis excepturi vel tempore perspiciatis nisi molestiae recusandae voluptas. Pariatur molestiae tempora laudantium id minima nulla, maxime perspiciatis error exercitationem laborum! Odio quibusdam placeat ipsum id consectetur. Doloribus praesentium ea fuga nulla aspernatur, vero, optio incidunt quidem, quod molestiae totam exercitationem minima! Fugit quasi, earum maiores deserunt expedita cumque quod facilis numquam distinctio! Voluptatibus officiis cupiditate minus esse aperiam dolor nesciunt neque tempore ullam odio nam unde fugiat saepe, rerum explicabo architecto autem ad perspiciatis temporibus cumque quod! Quo delectus molestiae sequi harum animi quidem hic officia natus dicta inventore! Maxime quia veniam doloremque totam at accusamus iusto nobis! Excepturi minima consequuntur dolore necessitatibus, quod cupiditate maxime laborum architecto nulla! Nostrum, iste perferendis! Nulla, qui praesentium laudantium temporibus maxime deserunt vero aliquid molestiae eveniet dolorem repellendus magnam eius at accusamus tenetur deleniti dolorum veritatis possimus facilis eum! Ex officia consequatur distinctio molestias vero omnis ipsa iusto laborum vel? Vitae voluptatibus adipisci ratione aspernatur possimus magni provident? Nesciunt ratione cumque eum doloremque doloribus perferendis blanditiis odit optio sed iure excepturi odio necessitatibus esse dolores, dolore autem delectus obcaecati molestiae cum, unde adipisci, et temporibus. Exercitationem eveniet illo harum ad laborum.</p>
    </section>
``` 


### External CSS
- External CSS: - In the external CSS, a CSS file will be created by using *.css * extension & that *CSS* file will be linked in the HTML file using &lt;link&gt; tag.

For example :-  This is an external.html file which links to style.css file


```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>External-CSS</title>
    <link rel="stylesheet" href="style.css">
</head>
``` 

This is a style.css file all the styling will be done here.

```
.After-CSS
{
  text-align: justify;
  color: #c71d1dd2;
}

#section
{
  background-color: #acc030b1;
}

.Para
{
  color: #43003c;
}
``` 


** But CSS is not much easier….**
> There is an algorithm called “specificity” used by browsers to decide which property should be displayed to the user which is applied on the elements


We will talk about it in upcoming blog…..till then just Keep calm.
 
Now,

Suppose you have a lot of span tags in your HTML document, you want to style them differently,
But due to the same source, the specificity will the same.

And the browser will render the second one for styling .

Why???

Because of most popular term of OOPS i.e., override. 

>Override means if there are two methods with the same name then the last one will be applied. 




```
<style>
    span
      {
        background-color: #f4aaaa;
        color:#0c0c0c;
      }
    span
      {
        background-color: #1682db;
        color:#d00505;
      }
   span
    {
        background-color: #70b5ee;
        color:#5c0404;
    }
  
  
   </style>
</head>
<body>
    <span>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nisi, impedit.</span>
    <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem, fugit.</span>
    <span>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Reprehenderit, sint!</span>
   
</body>
</html>

``` 

In this example, there are three &lt;span&gt;  and we want to apply different styling on all the &lt;span&gt; tags but due to the same source i.e. &lt;span&gt; only the last one will be applied on all the &lt;span&gt; tags.

# CSS selectors


CSS selectors are used to target the HTML elements for applying the CSS property. It can be done in different ways.

### Ways of Applying Selectors: -  

- Universal selector: - Universal selector is used to target all the elements present in the HTML document. It can be done by using asterisk (*).


```
	  <style>
		    *{
	        background-color: #eedec9;
            }


``` 

By using Universal Selector, the background color of the whole webpage will be changed because all the elements are targeted.


- Individual selector: - Individual selectors are those which target the elements individually or one by one. 


```
	 /* Individual Selectors */
	    
	      h1
          {
	        background-color: #6161e5;
	      }
	      h2
          {
	        background-color: #cc6e6e;
	      }
	      h3
          {
	        background-color: rgb(213, 200, 141);
	      }
	      p
          {
	        color:#ff09e6;
	      }

``` 

Here, all the &lt;h1&gt;,&lt;h2&gt;,&lt;h3&gt; and &lt;p&gt; tags are targeted where the browser will render these tags in the HTML document the styling will applied on that elements.



- Class and Id selector :- In class selector we use (.) with *class* name of elements and in* id *selector ,we use (#) with the id_name of the element.

> The main difference between Id and class selector is that, *id name* should be unique in the whole HTML document whereas* class name *can be same for elements.


```
  /* class and id selector selectors */
    .paragraph, #paragraph1
    {
        border-radius: 2px;
        border: 2px dotted #e71919;
        color: #6161e5;
        padding: 0px 20px 0px 20px;
        margin: 10px 80px 0px 80px;

    }
    .heading{
        text-align: center;
    }

``` 

In this,** .paragraph **denotes that it is a class name and** #paragraph1 **denotes that it is an Id-name.



- Combined selector  :-  combined selectors can be used where we wants to target multiple elements for the same styling.


```
	  table,th,td
            {
	            border: 1px solid black;
	            border-collapse: collapse;
	        }

``` 

In this we have a &lt;table&gt; ,&lt;th&gt; and &lt;td&gt; and we combined these elements and target them for the common border styling.



-   Direct child: - Direct child selector is used when we use nesting of elements that means if we use elements inside elements, it will become a hierarchy as like a tree. 


![blog3css.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668331671257/FpnR1hSUi.png align="left")


In above diagram, Parent node has two child node  i.e child node a and child node b. Child node A further has two child nodes but they are grandchildren to the root node(named as parent node in diagram).

> So, in direct selector we will use > sign to tell the browser that there is a hierarchy which is targeted to apply CSS on it.

```
<div>
    <h1 class="heading" >Selector List</h1>

    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nam at, ea consectetur aut deserunt, dolorum commodi quis sequi fugiat eum nesciunt
         <ol>
                <li>hello</li>
        </ol>
    </p>

    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis p>
    <ol>
        <li>universal selector </li>
        <li>individual selector </li>
        <li>class and id selector </li>
        <li>and selector (chained) </li>
        <li>combined selector </li>
        <li>inside an element </li>
        <li>direct child </li>
        <li>sibling  ~ or + </li>
    </ol>
    

   </div>

``` 

```
    div > ol > li {
        text-decoration:underline;
        color: #035a5a;

    }

``` 

In this selector, We want to target the grandchild of &lt;div&gt; so,we will target it by using its direct child i.e. &lt;ol&gt; 


- Inside an element: - In this selector, we will target the element inside an element, but it doesn’t matter whether that element is its direct child or not.  


```
<div>
    <h1 class="heading" >Selector List</h1>

    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
         <ol>
                <li>hello</li>
        </ol>
    </p>

    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis p>
    <ol>
        <li>universal selector </li>
        <li>individual selector </li>
        <li>class and id selector </li>
        <li>and selector (chained) </li>
        <li>combined selector </li>
        <li>inside an element </li>
        <li>direct child </li>
        <li>sibling  ~ or + </li>
    </ol>

``` 


```
/* inside element  */
    div li{
        color:#dc4e16 ;
        background-color: #000000; 
    }

``` 
> Here the &lt;li&gt; is not a direct child to &lt;div&gt; but it is targeted.


```
 div p,h1,li{
        color:#dc4e16 ;
        background-color: #000000; 
}
``` 

> Multiple elements inside an element can be targeted by using comma (,).




- and selector or Chained Selector: - This selector is totally based on “AND” concept of computer science that means if there are two variables and the values both is TRUE then the result will be true.


```
 <p class = "chain p1" >
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae, iure.
    </p>

 <p class="chain ">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Itaque, delectus.
    </p>
``` 


```
 /* Chained or "and" selector */
    p.chain.p1{
        color:#5f9ea0;
    }

```


It works if and only if an element has both classes *chain* and * p1*.

That means it only works on first &lt;p&gt; tag that contains both classes and id. It will not
target the other &lt;p&gt; tag which has only one class



Here, an another example 


```
<p class= "chain" id="p1">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, esse?
    </p>

``` 

```
 p.chain#p1{
        color:#dfdd42;
    }

``` 

It can also be done by using one class and one or both ids, but condition must be true.



- Sibling  Selector (~ or + ): - Sibling selectors are used when we want to target the sibling of an element.

> There are two ways of targeting siblings i.e by using tilde (~) and Addition (+) sign and both are used for different purpose.


```
<div>

        <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. At, earum.
        </p>
        <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eius, non?
        </p>
        <h1>
            This is Heading
        </h1>
        <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cupiditate, vero!
        </p>
        <h1>
            This is also a heading
        </h1>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, vitae?
        </p>
   </div>
``` 

All the &lt;p&gt; and &lt;h1&gt; tags are siblings here because they have same parent i.e. &lt;div&gt; tag


```
  p ~ h1
         {
            background-color: rebeccapurple ;
        }
``` 

Here, We targeted &lt;h1&gt; which is the sibling of &lt;p&gt; tag, there can be multiple  &lt;h1&gt; tags are present in HTML document but it will only target the sibling of &lt;p&gt; tag.

### Another method :-
 
Using Addition sign(+) :- In this, not all the siblings will get targeted but only the first sibling will be .


```
 <div>

        <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. At, earum.
        </p>
        <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eius, non?
        </p>
        <h1>
            This is Heading
        </h1>
        <h1>
            This is also a heading
        </h1>
        
        <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cupiditate, vero!
        </p>
        
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, vitae?
        </p>
   </div>
``` 

Here also, All the &lt;p&gt; and &lt;h1&gt; tags are siblings here because they have same parent i.e. &lt;div&gt; tag. but in &lt;p&gt; tag there are two &lt;h1&gt; tags are there.

```
  p + h1
         {
            background-color: rebeccapurple ;
        }
``` 
> Now, what will happen here ????

Only the first sibling &lt;h1&gt; of &lt;p&gt; tag will get targetet not both &lt;h1&gt; tags.



# Summary

In this article, We have learnt about the *Introduction of CSS* and *its selectors*. We learnt different types selectors.

Hope you'll like it. 

Many more Topics will be coming soon..... till then Bye Bye...


![bye-goodbye.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1668340200205/Fb2ha1iTS.gif align="left")

See you soon!!

Happy Learning!!







