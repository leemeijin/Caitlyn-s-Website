title: Simprints Challenge
cover_index: /assets/simprints.png
cover_detail: /assets/simprints.png
date: 2017-05-04 00:49:19
---
<!DOCTYPE html>
<html >
<head>
  <meta charset="UTF-8">
  <title>Simprints Cloud Coding Challenge</title>
  <script src="http://s.codepen.io/assets/libs/modernizr.js" type="text/javascript"></script>
<script type="text/javascript">var result = document.getElementById("success_message.textContent")

// Final Attempt (it seems to work)

function multiples_sum(){

var multiple_max = parseInt(document.getElementById('multiple_max').value),
multiple_1 = parseInt(document.getElementById('multiple_1').value),
multiple_2 = parseInt(document.getElementById('multiple_2').value),
multiple_3 = parseInt(document.getElementById('multiple_3').value)

var ans = [];
var k = 0;
var sum = 0

for (var i = 0; i < multiple_max; i++) {
  if (i % multiple_1  === 0 || i % multiple_2 === 0 || i % multiple_3  === 0) {
    ans.push(i);
    sum += i
  }
}

alert(sum);
document.getElementById("success_message").textContent = "Your Result: "+sum+" ";

}


// TERRIBLE INEFFICIENT ATTEMPT 2

/*
function multiples_sum(){

var multiple_max = parseInt(document.getElementById('multiple_max').value),
multiple_1 = parseInt(document.getElementById('multiple_1').value),
multiple_2 = parseInt(document.getElementById('multiple_2').value),
multiple_3 = parseInt(document.getElementById('multiple_3').value)

var sum_array = new Array();
var array_123 = new Array();

var sum_numbers = 0
var sum_overlaps = 0
var final_sum = 0


for (var i = 0; i < multiple_max; (i += multiple_1)) {
  sum_array.push(i);
}

for (var i = 0; i < multiple_max; (i += multiple_2)) {
  sum_array.push(i);
}

for (var i = 0; i < multiple_max; (i += multiple_3)) {
  sum_array.push(i);
}

for (var i = 0; i < multiple_max; i += ((multiple_1 + multiple_2) || (multiple_2 + multiple_3) || (multiple_1 + multiple_3)) {
  array_123.push(i);
}



for (var x = 0; x < sum_array.length; x += 1) {
  sum_numbers = (sum_numbers + sum_array[x])
}

for (var x = 0; x < sum_123.length; x += 1) {
  sum_overlaps = (sum_numbers + sum_123[x])
}

final_sum = sum_numbers - sum_overlaps

alert(sum);
document.getElementById("success_message").textContent = "Your Result: "+final_sum+" ";

}
*/

//ATTEMPT 1

/*function multiples_sum(){

  // Get the values
  var multiple_max = parseInt(document.getElementById('multiple_max').value),
  multiple_1 = parseInt(document.getElementById('multiple_1').value),
  multiple_2 = parseInt(document.getElementById('multiple_2').value),
  multiple_3 = parseInt(document.getElementById('multiple_3').value)

var sum = 0
for (var x=1; x <multiple_max; x++) {
  if (
    (multiple_1 && (multiple_1 % x)) ||
    (multiple_2 && (multiple_2 % x)) ||
    (multiple_3 && (multiple_3 % x)) )
{

    sum += x

  }
  }

alert(sum);
document.getElementById("success_message").textContent = "Your Result: "+sum+" ";

}
*/

</script>


  <link rel='stylesheet prefetch' href='http://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css'>
<link rel='stylesheet prefetch' href='http://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap-theme.min.css'>
<link rel='stylesheet prefetch' href='http://cdnjs.cloudflare.com/ajax/libs/jquery.bootstrapvalidator/0.5.0/css/bootstrapValidator.min.css'>

      <link rel="stylesheet" href="css/style.css">


</head>

<body>
  <div class="container">

    <div class="well form-horizontal" id="contact_form">
<fieldset>

<!-- Form Name -->
<legend>Simprints Cloud Coding Challenge!
<br></br>
<p> Give me a number (Max Number), and I can find the sum of all the multiples of other numbers up to but not including that number. </p>

</legend>

<!-- Text input-->

<div class="form-group">
  <label class="col-md-4 control-label">Max Number</label>
  <div class="col-md-4 inputGroupContainer">
  <div class="input-group">
  <input  id="multiple_max" placeholder="Maximum Number" class="form-control"  type="text">
    </div>
  </div>
</div>

<!-- Text input-->

<div class="form-group">
  <label class="col-md-4 control-label" >Enter another number </label>
    <div class="col-md-4 inputGroupContainer">
    <div class="input-group">
  <input id="multiple_1" placeholder="Multiple Number 1" class="form-control"  type="text">
    </div>
  </div>
</div>

<!-- Text input-->

<div class="form-group">
  <label class="col-md-4 control-label" >Enter another number</label>
    <div class="col-md-4 inputGroupContainer">
    <div class="input-group">
  <input id="multiple_2" placeholder="Multiple Number 2" class="form-control"  type="text">
    </div>
  </div>
</div>

<!-- Text input-->

<div class="form-group">
  <label class="col-md-4 control-label" >Enter another number</label>
    <div class="col-md-4 inputGroupContainer">
    <div class="input-group">
  <input id="multiple_3" placeholder="Multiple Number 3" class="form-control"  type="text">
    </div>
  </div>
</div>


<!-- Button -->
<div class="form-group">
  <label class="col-md-4 control-label"></label>
  <div class="col-md-4">
    <button type="default" class="btn btn-warning" onclick="multiples_sum()">Send <span class="glyphicon glyphicon-send"></span></button>
  </div>
</div>

<!-- Output Message -->
<div id="success_message">Thanks for using the program :) </div>


</fieldset>
</div>
</div>
    </div><!-- /.container -->
  <script src='http://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js'></script>
<script src='http://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/js/bootstrap.min.js'></script>
<script src='http://cdnjs.cloudflare.com/ajax/libs/bootstrap-validator/0.4.5/js/bootstrapvalidator.min.js'></script>

    <script src="js/index.js"></script>

</body>
</html>
