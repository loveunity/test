<head>
 <h1>get a number</h1>
</head>
<body onload="numbers()">
   
   <button id="joke-btn">Get Joke</button>
   <div id="joke" class="card">Click the "get a number" button</div>

    <script type="text/python" id="numbers">
    
    import numpy as np
    data = np.genfromtxt('sample_num.csv', delimiter = ',')
    print data
       
    </script>

</body>
