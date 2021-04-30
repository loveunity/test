<!DOCTYPE html>
<html>
  <head>    
  </head>
  <body>
    <input type="button" id='script' name="scriptbutton" value=" Run Script " onclick="goPython()">
     <!-- Ajax call -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/brython/3.8.8/brython.js" integrity="sha256-rA89wPrTJJQFWJaZveKW8jpdmC3t5F9rRkPyBjz8G04=" crossorigin="anonymous"></script> 

 <script src="https://cdnjs.cloudflare.com/ajax/libs/brython/3.8.8/brython_stdlib.js" integrity="sha256-Gnrw9tIjrsXcZSCh/wos5Jrpn0bNVNFJuNJI9d71TDs=" crossorigin="anonymous"></script> 
 <!-- Ajax call -->
 <script>
        function goPython(){
            $.ajax({
              URl: "numbers.py",
             context: document.body
            }).done(function() {
             alert('finished python script');;
            });
        }
</script>
</body>
</html>
