2.
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
    <style>
@import url(https://fonts.googleapis.com/css?family=Roboto+Condensed:400,400italic,300italic,300,700,700italic);
    
    * {
      font-family: 'Roboto Condensed', sans-serif;
    }
    
    h1 {
      font-weight: 500;
    }
    
    img {
      height: 400px;
      float: left;
      margin: 0 10px 0 0;
    }
    
    .fact {
      background-color: yellow;
    }
    
    footer {
      background-color: black;
      color: white;
      padding: 20px;
    }
  </style>
  <script>
    
    setTimeout(function () {
var getP = document.querySelector("p");
var getText = getP.firstChild;
var value = getText.nodeValue;

console.log(value);
      
          }, 0);

</script>

</head>
<body>
<div
     ><p>JavaScript is pretty powerful.</p>
</div>
</body>
</html>

3.

<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
    <style>
@import url(https://fonts.googleapis.com/css?family=Roboto+Condensed:400,400italic,300italic,300,700,700italic);
    
    * {
      font-family: 'Roboto Condensed', sans-serif;
    }
    
    h1 {
      font-weight: 500;
    }
    
    img {
      height: 400px;
      float: left;
      margin: 0 10px 0 0;
    }
    
    .fact {
      background-color: yellow;
    }
    
    footer {
      background-color: black;
      color: white;
      padding: 20px;
    }
  </style>
  <script>
    
    setTimeout(function () {
var getDiv = document.querySelector("div");
var getP = getDiv.firstChild;
var value = getP.textContent;

console.log(value);
      
          }, 0);

</script>

</head>
<body>
 <div
 ><p><em>JavaScript</em> is pretty <strong>powerful</strong>.</p>
</div>
</body>
</html>

4.

<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
  <script>
        setTimeout(function () {
    
var text;
var links;          
    var getUnorderedListArray = document.querySelectorAll("li");
    
   for (counter=0; counter < getUnorderedListArray.length; counter=counter+1) {
          
text = getUnorderedListArray[counter].textContent;
getUnorderedListArray[counter].removeChild(getUnorderedListArray[counter].firstChild);
var a = document.createElement("a");
var aClass = a.setAttribute("href", links[counter]);     
var newText = document.createTextNode(text);
a.appendChild(newText);
getUnorderedListArray[counter].appendChild(a);     
        }
          
              }, 0);
  </script>
</head>
<body>
<ul><li>London</li>
  <li>Paris</li>
  <li>New York</li>
</ul>
</body>
</html>

5.

<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
  <script>
        setTimeout(function () {
              
    var getUnorderedListArray = document.querySelectorAll("li");
    
   for (counter=1; counter < getUnorderedListArray.length; counter=counter+2) {
     

var liClass = getUnorderedListArray[counter].setAttribute("class", "highlight");        
        }
          
              }, 0);
  </script>
  <style>
    .highlight {
      background-color: orange;
    }
</head>
<body>
<ul>
  <li class="based-in">London</li>
  <li class="visited">San Francisco</li>
  <li>Paris</li>
  <li>Tokyo</li>
  <li class="going-to">New York</li>
</ul>
</ul>
</body>
</html>

6.

<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
  <style>
    .highlight {
      background-color: yellow;
    }
  </style>
  <script>
        setTimeout(function () {
   
  var sum =0;
  var images = [
  'http://valuestockphoto.com/freehighresimages/roast_veg_DSC2834.jpg',
  'http://valuestockphoto.com/freehighresimages/snowy_trees1995.jpg',
  'http://valuestockphoto.com/freehighresimages/nt_alice_springs140362.jpg',
  'http://valuestockphoto.com/freehighresimages/diwali_deepavali_DSC2292.jpg'
    ];
        var createImage = document.createElement("img");
        var imgSrc = createImage.setAttribute("src", images[sum]);
        var imgAlt = createImage.setAttribute("alt", "NO PICTURE");
        var imgWidth = createImage.setAttribute("width", "100%");
          
        function work () {  
        

        var imgSrc = createImage.setAttribute("src", images[sum]);
        document.body.appendChild(createImage);
        sum =  sum + 1
        if (sum>=images.length) {
          sum = 0
        }
        }

 var intervalID = window.setInterval(work, 5000);

              }, 0);
    
  </script>
</head>
<body>

</body>
</html>