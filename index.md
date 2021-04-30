  <html> 
 
        <head> 
            <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/brython/3.8.8/brython.js" integrity="sha256-rA89wPrTJJQFWJaZveKW8jpdmC3t5F9rRkPyBjz8G04=" crossorigin="anonymous"></script> 
        </head> 
 
        <body onload="brython()"> 
 
            <script type="text/python"> src="numbers.bry"></script>
                          
            def echo(event): 
                alert(document["zone"].value) 
             
            document["mybutton"].bind("click", echo) 
           
 
            <input id="zone"><button id="mybutton">click 19 !</button> 
 
        </body> 
 
    </html> 
