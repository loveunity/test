<!DOCTYPE html>
<html>
  <head> 
  <input type="button" id='script' name="scriptbutton" value=" Run Script " onclick="goPython()">
     <!-- Ajax call -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/brython/3.8.8/brython.js" integrity="sha256-rA89wPrTJJQFWJaZveKW8jpdmC3t5F9rRkPyBjz8G04=" crossorigin="anonymous"></script> 

 <script src="https://cdnjs.cloudflare.com/ajax/libs/brython/3.8.8/brython_stdlib.js" integrity="sha256-Gnrw9tIjrsXcZSCh/wos5Jrpn0bNVNFJuNJI9d71TDs=" crossorigin="anonymous"></script> 
     <!-- Ajax call -->   
  </head>
<body onload="brython()">
 
    <h1>Get a joke</h1>

    <button id="joke-btn">Get Joke</button>
    <div id="joke" class="card">Click the "get joke" button</div>

    <!-- Ajax call -->
    <script type="text/python" id="script13">
        from browser import document, ajax
		fuction goPython(){
		$.ajax({
		url:"numbers.py"
		context:document.body
		}).done(fuction(){
		alert('Finish");;
		});
		}        
    </script>

</body>

 
</body>
</html>
