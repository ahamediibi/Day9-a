<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>BOOTSTRAP TABLE</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.5.3/dist/css/bootstrap.min.css">

  <style>

    .my-container {
      font-weight: bold;
      font-size: 20px;
      width: 50%;
      margin: auto;
      text-shadow:2px 2px 5px gray;
    }

    .good {
      font-size: 25px;
      text-align: center;
      font-weight: bold;
      text-shadow:2px 2px 4px black;
    }
    
  .nice{
  text-shadow:2px 2px 5px white;
  box-shadow:4px 4px 10px black;
  }

  input[type=text] {
  border: 2px solid lightskyblue;
  box-shadow:4px 4px 10px lightskyblue;
}

input[type=email] {
  border: 2px solid lightskyblue;
box-shadow:4px 4px 10px lightskyblue;
}

.custom-select{
  font-weight: bold;
  border: 2px solid lightskyblue;
box-shadow:4px 4px 10px lightskyblue;
}
  </style>

</head>

<body>
  <h1 class="container my-container p-2 good text-success w-25 text-shadow">WELCOME TO DYNAMIC TABLE</h1>
  <br>
  <div class="container my-container p-1 text-shadow">
    <div class="row">
      <div class="col-lg-6 offset-lg-3 col-md-8 offset-md-2 col-sm-10 offset-sm-1">
        <form id="myForm">
          <div class="form-row">
            <div class="form-group col-md-6">
              <label for="first-name">First Name</label>
              <input id="first-name" class="form-control" type="text" name="first-name">
            </div>
            <div class="form-group col-md-6">
              <label for="last-name">Last Name</label>
              <input id="last-name" class="form-control" type="text" name="last-name">
            </div>
          </div>

          <div class="form-group">
            <label for="email">Email</label>
            <input id="email" class="form-control" type="email" name="email">
          </div>
          <div class="form-group">
            <label for="mobile">Mobile</label>
            <input id="mobile" class="form-control" type="text" name="mobile">
          </div>
          <div class="form-group">
            <label for="address-1">Address Line 1</label>
            <input id="address-1" class="form-control" type="text" name="address-1">
          </div>
          <div class="form-group">
            <label for="address-2">Address Line 2</label>
            <input id="address-2" class="form-control" type="text" name="address-2">
          </div>
          <div class="form-row" >
            <div class="form-group col-md-6" >
              <label for="district" >District</label>
              <select name="district" id="district" class="custom-select">
                <option value="CH">Chennai</option>
                <option value="CBE">Coimbatore</option>
                <option value="MD">Madurai</option>
                <option value="TR">Trichy</option>
                <option value="TC">Tuticorin</option>
                <option value="RM">Ramanathapuram</option>
                <option value="DG">Dindugal</option>
              </select>
            </div>
            <div class="form-group col-md-6">
              <label for="state">State</label>
              <select name="state" id="state" class="custom-select">
                <option value="TN">Tamil Nadu</option>
                <option value="KA">Karnataka</option>
                <option value="KL">Kerala</option>
                <option value="MB">Mumbai</option>
                <option value="UP">Uttar Pradesh</option>
                <option value="DH">Delhi</option>
                <option value="Rj">Rajastan</option>
              </select>
            </div>
          </div>
          <button type="submit" class="nice btn btn-success btn-block">Submit</button>
        </form>
        <div id="successMessage" class="mt-3 text-center" style="display: none;">
          <h4>Form submitted successfully!</h4>
          <p>Thank you for your submission.</p>
        </div>
      </div>
    </div>
  </div>

  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.5.3/dist/js/bootstrap.bundle.min.js"></script>
  <script>
    const form = document.getElementById('myForm');
    const successMessage = document.getElementById('successMessage');

    form.addEventListener('submit', (e) => {
      e.preventDefault();
      successMessage.style.display = 'block';
      form.reset();
    });
  </script>

</body>

</html>
