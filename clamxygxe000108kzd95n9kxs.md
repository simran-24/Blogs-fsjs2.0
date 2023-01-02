# Dive into Pseudo-classes

# Pseudo classes 

Pseudo-classes are used on some state of HTML elements to put styling on it and it contain the *Keywords* which have some pre-defined meaning in CSS.

In pseudo-class, it is mandatory to use (:) colon after the element or tag on which the developer wants to put styling. 

## Syntax :- 

**element :<pseudo-class>**
{
     css-property1;
     css-property2;
     css-property3;
             ...
             ...
}

# Characterize Pseudo classes based on their usage


The pseudo -classes mainly divided into four parts based on uses: - 

-  Used for linking
- 	Used on forms
- 	Used on Selectors
- 	Used for variable

## Used for Linking :-  

These pseudo-classes are used on links mainly, that means these classes are used to put styling on some state of a tags which contains the attribute *href* in it. 

These classes are :-

-     :active
-     :link
-     :any-link
-     :visited
-     :hover


### :active :-

 This pseudo-class will work when an event happen on an element, matches the state of the class. In brief, we can say that when a link becomes active by clicking  by mouse then the *:active* class will start working.
  
 ** Syntax : - a:active**
 {
 css-property1;
css-property2;
css-property3;
        ….
        ….
}


**Note:- ** the Link will be called as active when a user just click on it. If the user click out of the link it    will disappear as the link will be opened.
   

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/BaVdEJE?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>


###   :link :-

This pseudo-class will work when the element contains the *href *that means the styling will be done on all the links .but after visiting the link, color of the text will get changed.

**Syntax: - a:link**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="link" src="https://codepen.io/simran-24/embed/zYaPaXW?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true"></iframe>



### :any-link :- 

This pseudo-class will give styling to the link either they're visited or not. The text-color will not get changed until and unless we give the styling on* :visited* class. It will stop doing work after *:visited* class 

**Syntax: - a:any-link**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="any-link" src="https://codepen.io/simran-24/embed/LYrOrKM?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

### :visited :- 

This pseudo-class will not put styling on the link until it is visited by the user.

**Syntax: - a:visited**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="visited" src="https://codepen.io/simran-24/embed/MWXOBWO?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>


### :hover  :-

This pseudo class will work on state of hover that means when a user hover the mouse on the targeted element then it will show some styling on it.


**Syntax: - a:hover**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 


<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/GRGOBJg?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>


### Source Code :- 

<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/OJEjGzq?default-tab=html&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">

</iframe>


## Used on Forms:-
These pseudo-classes basically developed to provide some special features to the forms. 
> Let’s Suppose , a client required a form which need to take input from the user for some fields and for some other fields they want to show the field but don’t required any input from the user.

**How can a developer create that form???**
   
The answer is ,by using Pseudo-classes.

These classes are :
- :checked
- :focus
- :disabled
- :enabled
- :required
- :optional
- :read-write
- :read-only
- :valid
- :invalid
- :in-range
- :out-of-range
- :default

### :checked :-

In this pseudo-class, the CSS-styling will target those elements which contains the keyword “*checked* ” in it. The *checked* keyword will treat the value as default value.

**Syntax: - element:checked**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="checked" src="https://codepen.io/simran-24/embed/jOKapqw?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

### :focus :-

 :focus class will start  working  when an element got triggered by an event i.e mouse-click , giving input through keyboard. When the focus will shift to the element , the CSS will target that element instantly.

**Syntax: - element:focus**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 


<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/NWzwBbp?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>

### :disabled :-

*disabled* is a keyword that is used whenever we don’t want to take input from the user but the option must be shown to the user to cross-verify the details.

:disabled class is used to target that element for putting some styling on it.

Let's Assume :- A developer is creating a Government form (Indian) ,so the main requirement is to make the by default value of country as “India” and make the option disable so that any user can’be able to change the value.

**Syntax: - element:disabled**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="disabled" src="https://codepen.io/simran-24/embed/rNKYrjr?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>

### :enabled :- 

All the element called as enabled until the developer provides a disabled value. The element can also be enable by clicking on them.

**Syntax: - element:enabled**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="enabled" src="https://codepen.io/simran-24/embed/ZERajyR?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>


### :required :-

*required* is also a keyword which target the fields of the form, which is required to be filled before submitting, if the user don’t fill that field, the form will not get submitted and also it will show the alert message.

> :required class will target that element which contains the keyword “*required*” and put the styling on it

**Syntax: - element:required**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 


<iframe height="300" style="width: 100%;" scrolling="no" title="required" src="https://codepen.io/simran-24/embed/vYrWaWN?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  </iframe>

### :optional :- 

*optional* is a keyword which target the fields of the form, which is not required to be filled before submitting, if the user don’t fill that field, the form will get submitted and it used for feedback purpose mainly. 

> :optional class will target that element which contains the keyword “*optional*” and put the styling on it

**Syntax: - element:optional**{ css-property1;
css-property2;
css-property3;
        ….
        ….}


### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="optional" src="https://codepen.io/simran-24/embed/wvXPxpd?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

### :read-only :-

*readonly* keyword is used for making the values as readable only. In this, the user can’t make changes to the values. but we can make changes by going one step back.

> :read-only class will target the element which contains the readonly keyword

**Syntax: - element:read-only**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="read-only" src="https://codepen.io/simran-24/embed/JjZOBvQ?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

### :read-write :-

read-write is the class  that makes the user to read the content of the targeted element as well as edit the content.

**Syntax: - element:read-write**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 
<iframe height="300" style="width: 100%;" scrolling="no" title="read-write" src="https://codepen.io/simran-24/embed/LYrOBgY?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>


### :valid & :invalid :-

:valid class put styling on that element which contains the valid value. whereas :invalid class put styling on that element which contains invalid values in it.

> Example :- we have three input types i.e., text, number and email, all fields are valid until & unless we explicitly enter some invalid value in fields as like we set a numeric value in input email then the styling will be shown of :invalid class.

**Syntax: - element:valid**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

**Syntax: - element:invalid**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="VALID-Invalid" src="https://codepen.io/simran-24/embed/qBKVyLB?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </a>.
</iframe>


### :in-range :- 

For using “in-range” pseudo-class , we need to provide the min and max attribute in the element , so that the CSS will target that element which has the value within the given range.

**Syntax: - element:in-range**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="in-range" src="https://codepen.io/simran-24/embed/xxzPJeK?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>

### :out-of-range :-

For using “out-of-range” pseudo-class , we need to provide the min and max and value attribute in the element, so that the CSS will target that element which has the value out of the given range.

**Syntax: - element:out-of-range**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="out-of-range" src="https://codepen.io/simran-24/embed/poKdZXx?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>

### :default :- 

: default class will target all the element which contains the keyword “selected” or “checked” in it. There can  be multiple selected or checked in a document.  
First, we will understand the working of “selected” Keyword .

Selected :- By using this keyword, we can make a value as default as we did above using* checked*.

> Example :- There are a lot of countries in the world, and we want to put an option to select the country but we don’t want to a blank selection as default. So, we will use the keyword selected. 

**Syntax: - element:default**{ css-property1;
css-property2;
css-property3;
        ….
        ….}

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/NWzwLKY?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  
</iframe>


The above example contains only one default value. It's been selected by default.

But if we create a checkbox and we want multiple default values in it we can do so by using checked keyword

*:default* class will put styling on all the elements which contains the “selected” or “checked” keyword


> **Note **: If there is Submit button in your Form, it will be count as default and :default class will reflect on this button too.

### Example 

<iframe height="300" style="width: 100%;" scrolling="no" title="default" src="https://codepen.io/simran-24/embed/RwJjYPp?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>


# Summary  :-

In this article, We have talked about pseudo-classes and the characterization of pseudo-classes on th basis their usage. We have seen many example of pseudo-classes . We explained only two characterizations , other two parts will be covered in next article .

## Source Code Link :- 

Github :- https://github.com/simran-24/12-Nov-fsjs2.0


Hope it was Helpful!!

Happy Learning!!


![winnie-the-pooh-see-you.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1668802454720/ivkvpOl0A.gif align="left")

See you Soon.......


