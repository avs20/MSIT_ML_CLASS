Errors :

1. X is not subscriptable. 

What is Subscriptable. This refers to object which are used with  **[]**. We have see a few of them where using [] is allowed. 

*  Strings
*  Lists
*  Dictionaries
*  Tuples 

So when this error comes, *this means you are using [] on some object which is not one of these.*

How to solve ?
Look at the error line as see which object is using [] and then think about why this is wrong. 

Most common issue of this error is in form 
*DictReader object is not subscriptable* 

DictReader is a type of file object and not one of these. So don't use **[]** with this.

Use the code of dictreader like 

```
for row in trip_reader:
    first_trip = row
    break
```
So row already contains the data from the **trip_reader** object. 


2. X is not callable 

We have used the word *call* only once when we *call* a function. 
So when we see the error *X is not callable* then this means that *X is not a function but we are using it as a function*

Functions are identified by using *()* after it's name. 

so check the error line and see where *()* is written and confirm that it's a function. If it's not remove the *()*


*3. Assertion Error*

This error will come when the output of your function (the value you are returning) is not as expected. 

The correct values are presented in the *tests* variable below the function code. 

So to compare the values, *print what your function is returning* and check if the values returned are same as in the *tests* variable. If not modify your code to return those values correctly. 