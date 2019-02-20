# competition-estimator
<!doctype html>
<html lang="en">

<head>
  <title>competition-estimator</title>
  <!-- Font Awesome -->
  <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.7.0/css/all.css">
  <!-- Bootstrap core CSS -->
  <link href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.2.1/css/bootstrap.min.css" rel="stylesheet">
  <!-- Material Design Bootstrap -->
  <link href="https://cdnjs.cloudflare.com/ajax/libs/mdbootstrap/4.7.3/css/mdb.min.css" rel="stylesheet">

</head>

<body>
  <main class="container-fluid">

    <h1>JavaScript for competition-estimator</h1>
    <h3>Right-click / Inspect, then select console</h3>

    <p>Enter your name:
      <input id="guest" type="text" value="Eden">
    </p>

    <p>Enter first number:
      <input id="students" type="number" value="7">
    </p>

    <p>Enter second number:
      <input id="positions" type="number" value="12">
    </p>

    <button id="clicker" class="btn btn-primary">Click me!</button>

    <p id="result"></p>

  </main>

  <script>
    console.log('SCRIPT START')
    console.log('Declare testable functions.....................')
    function add(x, y) {
      return x + y
    }
    console.log('Defined add=' + add)
    console.log('Declare event listeners .......................')
    document.getElementById('clicker').addEventListener('click', function () {
      const s = document.getElementById('guest').value
      const i = parseInt(document.getElementById('firstNumber').value)
      console.log('i=' + i)
      const j = parseInt(document.getElementById('secondNumber').value)
      console.log('j=' + j)
      const ans = s + ', your sum is ' + add(i, j) + '.'
      document.getElementById('result').innerHTML = ans
    })
    console.log('SCRIPT END')
  </script>

  <!-- JQuery -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  <!-- Bootstrap tooltips -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.4/umd/popper.min.js"></script>
  <!-- Bootstrap core JavaScript -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.2.1/js/bootstrap.min.js"></script>
  <!-- MDB core JavaScript -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/mdbootstrap/4.7.3/js/mdb.min.js"></script>
</body>

</html>
