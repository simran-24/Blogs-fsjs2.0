# Let's Play with <Table>

Firstly, We need to understand that actually what a table is.

So, Let's Start

### What is Table????

A table is a combination of rows and columns. It is a better way to share the information in tabular form. because it can be understood by any person whether they are professional or not.

Sometimes, we need to share the information on the website in tabular form.

For that purpose, we will use the &lt;**table&gt;** tag in our HTML document. It is a container tag.

> A container tag means that the tag needs to be closed by using the closing tag &lt;/&gt;.

```
<table> 
     
</table>
```

But in the above syntax, there is a problem in that, it can't do anything on the webpage because we need to some use more tags for adding rows and columns in the table.

## List of tags used in &lt;table&gt;


### &lt;tr&gt; 

tr stands for "Table row". It is used to define the row of the table. By using rows, we can add data horizontally.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1670310537639/JV7VjEuYp.png align="left")



### &lt;th&gt; 

th stands for "Table Head". It defines the heading of the table columns. In columns, 
we add the data in vertical manner.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1670311920237/4XYqWHwZQ.png align="left")

**Syntax**


```
<table>
        <tr>
           <th>Heading</th>  
        </tr>
</table
``` 

** Example :-**

 Using one row having table headings (three columns).
 

<iframe height="300" style="width: 100%;" scrolling="no" title="Table tr and th" src="https://codepen.io/simran-24/embed/mdKaodY?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>



###  &lt;td&gt; 

 td stands for "Table data". It is used to get added the data into rows according to the headings. ***&lt;th&gt;*** and ***&lt;td&gt;*** works in a same way but it is good practice to use ***&lt;th&gt; *** for table headings and***&lt;td&gt;*** for content or data into the rows.

**Syntax :- **


```
 <table>
        <tr>
            <th>Heading 1</th>
            <th>Heading 2</th>
            <th>Heading 3</th>
        </tr>
        <tr>
            <td>Table Data</td>
            <td>Table Data</td>
            <td>Table Data</td>
        </tr>

``` 


**Example :- **

<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/jOKXJMy?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>


### &lt;caption&gt; 

caption is a container tag used in table to give the caption to the table. It shows the caption outside the table boundary

 **Syntax** 

```
<table>
        <caption>Caption to show here</caption>
        <tr>
            <th>Heading 1</th>
            <th>Heading 2</th>
            <th>Heading 3</th>
        </tr>
        <tr>
            <td>Table data</td>
            <td>Table data</td>
            <td>Table data</td>
        </tr>
    </table>
``` 
**Example : -**

<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/jOKXJZw?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>


### &lt;thead&gt; 

 thead is a tag which is used as a header of the table. It groups the header.

### &lt;tfoot&gt; 

 tfoot is a tag which is used as a footer of the table. It is used to make the sum up of the data of the table .

### &lt;tbody&gt; 

tbody is a tag which is used to add the content of the table. It contains the data of the table.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1670330089110/zJxQHYxYr.png align="left")

**Syntax : -**


```
 <table>
        <caption>Caption Here</caption>
        <thead>
            <tr>
                <th>Heading 1</th>
                <th>Heading 2</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Data here </td>
                <td>Data here</td>
            </tr>
            <tr>
                <td>Data here</td>
                <td>Data here</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <th>Footer </th>
                <th>Footer</th>
            </tr>
        </tfoot>
    </table>
``` 
 **Example : -**

<iframe height="300" style="width: 100%;" scrolling="no" title="table thead" src="https://codepen.io/simran-24/embed/rNKoXZB?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
 </iframe>



# Attributes used in Table 


### span 

 span is used to group one or more cell. It can be either row or column. 

> For grouping cells horizontally, we can use row-span and for grouping cells vertically we can use  col-span


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1670337693038/V4sctoFUf.png align="left")

**Syntax :- **

```
 <table>
            <tr>
                  <th colspan="Value">Table Heading/Data </th>
            </tr>
            <tr>
                  <td rowspan="Value">Table Heading/Data</td>
      
``` 
** Example :- **
<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/simran-24/embed/OJEdJPL?default-tab=html%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>

### scope

scope has no visual impact on the table but it is used in &lt;th&gt; tag to get know whether the heading is for row or column. In simple terms, scope is used for screen readers to let them know whether the head is for row or column.

**Syntax :- **


```
<table>
        <tr>
                <th scope = "row | column | colgroup | rowgroup"> </th>
        </tr>
</table>
``` 

#Summary 

In this article, we have gone through the &lt;table&gt; tag and all its underlying tags i.e. &lt;tr&gt; , 
&lt;th&gt; ,&lt;td&gt; ,&lt;thead&gt; ,&lt;tbody&gt; , &lt;tfoot&gt; ,&lt;caption&gt; .We also talked about its main attributes i.e. scope and span. 

Hope it was helpful.

Happy Learning!

![tenor.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1670338564313/Ryrx-Jwb2.gif align="left")

LinkedIn Profile :- https://www.linkedin.com/in/simran-8b7310249/

Github Profile :- https://github.com/simran-24
   







