<input type = “button” id=”b1″ value=”1″>

<script>

$(document).ready(function(){

$("#b1").click(function(){

$.ajax({

method: "GET",

url: "numbers.py",

data: {"place" : value},

dataType: "text",

success: function(result){

var data=JSON.parse(result);

console.log(result);

}

});

});

</script>
