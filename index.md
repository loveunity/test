<head>
<!-- Ajax call -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/brython/3.8.8/brython.js" integrity="sha256-rA89wPrTJJQFWJaZveKW8jpdmC3t5F9rRkPyBjz8G04=" crossorigin="anonymous"></script> 

<script src="https://cdnjs.cloudflare.com/ajax/libs/brython/3.8.8/brython_stdlib.js" integrity="sha256-Gnrw9tIjrsXcZSCh/wos5Jrpn0bNVNFJuNJI9d71TDs=" crossorigin="anonymous"></script> 
 <!-- Ajax call -->
</head>
<body onload="brython()">
    <h1>get a number</h1>

    <button id="joke-btn">Get Joke</button>
    <div id="joke" class="card">Click the "get a number" button</div>

     <h1>Numbers</h1>
    <script type="text/python" id="numbers">
    
    import numpy as np
    data = np.genfromtxt('sample_num.csv', delimiter = ',')
    print data
       
    </script>

</body>
