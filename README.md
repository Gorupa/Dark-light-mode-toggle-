<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Your head content, meta tags, stylesheets, etc. --> 

  <!-- CSS for dark/light mode -->
  <style>
    /* Place your existing styles here */ 

    /* Dark/Light Mode Toggle */
    #modeSwitch {
      display: none;
    } 

    .switch {
      position: relative;
      display: inline-block;
      width: 60px;
      height: 34px;
    } 

    .switch input {
      opacity: 0;
      width: 0;
      height: 0;
    } 

    .slider {
      position: absolute;
      cursor: pointer;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: #ccc;
      -webkit-transition: .4s;
      transition: .4s;
    } 

    .slider:before {
      position: absolute;
      content: "";
      height: 26px;
      width: 26px;
      left: 4px;
      bottom: 4px;
      background-color: white;
      -webkit-transition: .4s;
      transition: .4s;
    } 

    input:checked + .slider {
      background-color: #2196F3;
    } 

    input:focus + .slider {
      box-shadow: 0 0 1px #2196F3;
    } 

    input:checked + .slider:before {
      -webkit-transform: translateX(26px);
      -ms-transform: translateX(26px);
      transform: translateX(26px);
    } 

    /* Dark mode styles */
    body.dark-mode {
      background-color: #333;
      color: #fff;
    }
  </style>
</head>
<body> 

  <!-- Dark/Light Mode Toggle -->
  <div class="mode-toggle">
    <label class="switch">
      <input type="checkbox" id="modeSwitch">
      <span class="slider round"></span>
    </label>
  </div> 

  <!-- The rest of your HTML content --> 

</body>
</html>
