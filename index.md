  <html> 
 
        <head> 
            <script type="text/javascript" src="src="https://cdnjs.cloudflare.com/ajax/libs/brython/3.8.8/brython.js" integrity="sha256-rA89wPrTJJQFWJaZveKW8jpdmC3t5F9rRkPyBjz8G04=" crossorigin="anonymous"></script> 
        </head> 
 
        <body onload="brython()"> 
 
            <script type="text/python"> 
            from browser import document, alert
            
            import numpy as np
            data = np.genfromtxt('sample_num.csv', delimiter = ',')
            print (data) 
            
            def echo(event): 
                alert(document["zone"].value) 
             
            document["mybutton"].bind("click", echo) 
            </script> 
 
            <input id="zone"><button id="mybutton">click !</button> 
 
        </body> 
 
    </html> 
