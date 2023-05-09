### Output should be :- 
![image](https://github.com/YashasviCodes/Web-Dev/assets/124666305/f7d7c825-6a29-4574-9cb4-e4e8cad6da76)

###Measurements :- 
[laos flagmeasurements.pdf](https://github.com/YashasviCodes/Web-Dev/files/11432444/laos.flag.measurements.pdf)

#### code:- 
```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>CSS Flag Project</title>
  <style>
    /* Write your CSS Code here */
    /* outter most div */
    
    /* main red part */
    .flag{
        background-color: rgb( 206,17,38 );
        height:600px;
        width:900px;
        position:relative; /*because blue box is relativily placed with this block*/
    }
    
    /* 'The Flag' part */
    .flag > p{
        color:white;
        font-size: 5rem;
        margin:0px;
        text-align: center;
        /* position:relative; */
    }

    /* center blue part */
    .flag > div{
        background-color: rgb(0,40,104);
        height:300px;
        width:900px;
        position: absolute; /*because this is relative to red box, and the white box is relative to this block*/
        top: 150px;
        
    }

    /* circle white part */
    .flag > div > div {
        background-color: white;
        height:200px;
        width:200px;
        border-radius : 50%;
        position:relative;  /*this is relatively placed with above '.flag > div' i.e blue box */
        left:350px;
        top:50px;
    }

    /* 'of Laos' text part*/
    .flag > div > div > p{
        text-align:center;
        color:black;
        font-size: 5rem;
        margin:0;
    }

    /* 0,40,104 - blue
       206,17,38 - redish 
    */
  </style>
  
</head>

<!-- 
  IMPORTANT! Do not change any HTML
Don't add any classes/ids/elements 
Use what you know about combining selectors 
and CSS specificity instead.
Hint 1: The flag is 900px by 600px and the circle is 200px by 200px.
Hint 2: You can use CSS inspection to get the colors from
https://appbrewery.github.io/flag-of-laos/
-->
 
<body>
  <div class="flag"> <!--red part--> <!-- height : 600, width:900 -->
    <p>The Flag</p>  <!--do not do coloring in p, because it will help is to place the text at right place-->
    <div>  
      <div>
        <p>of Laos</p> 
      </div>
    </div>
  </div>
</body>

</html>


<!-- IMPORTANT Takeaways :- 

  1. while placing text content inside a div, always place it in a 'p' tag, because that will help us place the text to its correct position.
  2. for absoute positioning, ancestor must be relative or absolute;

-->

```
