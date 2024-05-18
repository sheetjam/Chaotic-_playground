<!DOCTYPE html>
<html>
<head>
  <title>grid practice</title>

</head>
<body>
  <div 
  style="display: grid;
  grid-template-columns: 100px 100px 200px;
  margin-bottom: 15px;">
    <div style="background-color: blue;">
    100px
    </div>
      
    <div style="background-color: aqua;">
      100px
      <p>text</p>
    </div>
    <div style="background-color: blueviolet;">
      200px
    </div>
  </div>
  <div 
  style="display: grid;
  grid-template-columns: 100px 100px ;">
    <div style="background-color: blue;">
    div 1
    </div>
      
    <div style="background-color: aqua;">
      div 2
      <p>text</p>
    </div>
    
  </div>



  <div 
  style="display: grid;
  grid-template-columns: 100px 1fr ;
  margin-bottom: 15px;
  margin-top: 15px;">
    <div style="background-color: blue;">
    100px
    </div>
      
    <div style="background-color: aqua;">
      1fr
      <p>text</p>
    </div>

  </div>


  <div 
  style="display: grid;
  grid-template-columns: 100px 1fr 2fr;
  margin-bottom: 15px;
  margin-top: 15px;">
    <div style="background-color: blue;">
    100px
    </div>
      
    <div style="background-color: aqua;">
      1fr
      <p>text</p>
    </div>
    <div style="background-color: brown;">
      2fr
    </div>

  </div>



  <div 
  style="display: grid;
  grid-template-columns: 100px 1fr 1fr;
  margin-bottom: 15px;
  margin-top: 15px;">
    <div style="background-color: blue;">
    100px
    </div>
      
    <div style="background-color: aqua;">
      1fr
      <p>text</p>
    </div>
    <div style="background-color: brown;">
      1fr
    </div>

  </div>


</body>

</html>
