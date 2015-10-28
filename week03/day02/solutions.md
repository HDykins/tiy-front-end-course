1.
<!DOCTYPE>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
  <style>
    .first {
      background-color: yellow;
    }
  </style>
  <script>

    setTimeout(function () {
      
var unorderedNode = document.querySelector("ul");
var listNode = unorderedNode.firstChild;
var listClassFirst = listNode.setAttribute("class", "first");

          }, 0);

  </script>
</head>
<body>
  <button>Hello World</button>
<ul
    ><li>London</li>
  <li>Paris</li>
  <li>Tokyo</li>
  <li>New York</li>
</ul>
</body>
</html>

2.
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
  <script>
 setTimeout(function () {
       // Given the following HTML fragment:
//   <div>
 // <p id="latest"><strong>Friday</strong> is finally here.</p>
 // <p>In addition the weather is sunny today.</p>
//</div>

// Get the text content:
var text = document.getElementById("latest").textContent;
// |text| is set to "This is some text".

// Set the text content:
document.getElementById("latest").textContent = 'Monday is finally here.';
// The HTML for divA is now:
//   <div id="divA">This is some text</div>
                }, 0);
</script>

</head>
<body>
<div>
<p id="latest"><strong>Friday</strong> is finally here.</p>
  <p>In addition the weather is sunny today.</p>
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
var h1 = document.createElement("h1");
var h1Text = document.createTextNode("The Shard");
h1.appendChild(h1Text);
document.body.appendChild(h1);
      
      
      
      var h2 = document.createElement("h2");
var h2Text = document.createTextNode("The tallest building in Western Europe.");
h2.appendChild(h2Text);
document.body.appendChild(h2);
      
      
      
            var img = document.createElement("img");
var imgsrc = img.setAttribute("src", "https://upload.wikimedia.org/wikipedia/commons/thumb/0/07/The_Shard_from_the_Sky_Garden_2015.jpg/480px-The_Shard_from_the_Sky_Garden_2015.jpg");
      var imgalt = img.setAttribute("alt", "image of the shard")
document.body.appendChild(img);
      
      
      
      var firstParagraph = document.createElement("p");
      var firstParagraphText = document.createTextNode("The Shard, also referred to as the Shard of Glass, Shard London Bridge and formerly London Bridge Tower, is an 95-storey skyscraper in Southwark, London, that forms part of the London Bridge Quarter development. ");
      firstParagraph.appendChild(firstParagraphText);
      var span = document.createElement("span");
var spanClass = span.setAttribute("class", "fact");
var firstParagraphText = document.createTextNode("The Shard's construction began in March 2009");
            span.appendChild(firstParagraphText);
            firstParagraph.appendChild(span);
      var firstParagraphText = document.createTextNode("; it was topped out on 30 March 2012 and inaugurated on 6 July 2012. Practical completion was achieved in November 2012. The tower's privately operated observation deck, the View from the Shard, was opened to the public on ");
      firstParagraph.appendChild(firstParagraphText);
      var strong = document.createElement("strong");
var firstParagraphText = document.createTextNode("1 February 2013");
            strong.appendChild(firstParagraphText);
            firstParagraph.appendChild(strong);
            var firstParagraphText = document.createTextNode(".");
      firstParagraph.appendChild(firstParagraphText);
      document.body.appendChild(firstParagraph);
      
      
      
            var secondParagraph = document.createElement("p");
            var span = document.createElement("span");
var spanClass = span.setAttribute("class", "fact");
var secondParagraphText = document.createTextNode("Standing 309.6 metres (1,016 ft) high");
span.appendChild(secondParagraphText);
secondParagraph.appendChild(span);
      var secondParagraphText = document.createTextNode(", the Shard is currently ");
            secondParagraph.appendChild(secondParagraphText);
      var span = document.createElement("span");
var spanClass = span.setAttribute("class", "fact");
var secondParagraphText = document.createTextNode("the joint 92nd tallest building in the world");
span.appendChild(secondParagraphText);
secondParagraph.appendChild(span);
      var secondParagraphText = document.createTextNode(" and the fourth tallest building in Europe and the tallest building in the European Union. It is also the second-tallest free-standing structure in the United Kingdom, after the concrete tower at the Emley Moor transmitting station. The glass-clad pyramidal tower has 72 habitable floors, with a viewing gallery and open-air observation deck on the ");
            secondParagraph.appendChild(secondParagraphText);
            var span = document.createElement("span");
      var spanClass = span.setAttribute("class", "fact");
var secondParagraphText = document.createTextNode("72nd floor");
span.appendChild(secondParagraphText);
secondParagraph.appendChild(span);
      var secondParagraphText = document.createTextNode(", at a height of ");
            secondParagraph.appendChild(secondParagraphText);
      var span = document.createElement("span");
      var spanClass = span.setAttribute("class", "fact");
var secondParagraphText = document.createTextNode("244.3 metres (802 ft)");
span.appendChild(secondParagraphText);
secondParagraph.appendChild(span);
      var secondParagraphText = document.createTextNode(". It was designed by the Italian architect Renzo Piano and replaced Southwark Towers, a 24-storey office block built on the site in ");
            secondParagraph.appendChild(secondParagraphText);
      var span = document.createElement("span");
      var spanClass = span.setAttribute("class", "fact");
var secondParagraphText = document.createTextNode("1975");
span.appendChild(secondParagraphText);
secondParagraph.appendChild(span);
      var secondParagraphText = document.createTextNode(". The Shard was developed by Sellar Property Group on behalf of LBQ Ltd, and is jointly owned by Sellar Property and the State of Qatar.");
            secondParagraph.appendChild(secondParagraphText);
      document.body.appendChild(secondParagraph);
      
      
      
      var unorderedList = document.createElement("ul");
      var list1 = document.createElement("li");
var listText = document.createTextNode("Cost: ");
      list1.appendChild(listText);
         var span = document.createElement("span");
        var spanClass = span.setAttribute("class", "fact");
      var secondListText = document.createTextNode("~£435 million");
span.appendChild(secondListText);
      list1.appendChild(span);
unorderedList.appendChild(list1);
      
      var list1 = document.createElement("li");
var listText = document.createTextNode("Completed: ");
      list1.appendChild(listText);
         var span = document.createElement("span");
        var spanClass = span.setAttribute("class", "fact");
      var secondListText = document.createTextNode("July 2012");
span.appendChild(secondListText);
      list1.appendChild(span);
unorderedList.appendChild(list1);
      
            var list1 = document.createElement("li");
var listText = document.createTextNode("Opening: ");
      list1.appendChild(listText);
         var span = document.createElement("span");
        var spanClass = span.setAttribute("class", "fact");
      var secondListText = document.createTextNode("1 February 2013");
span.appendChild(secondListText);
      list1.appendChild(span);
unorderedList.appendChild(list1);
            document.body.appendChild(unorderedList);
      
      
      
var thirdParagraph = document.createElement("p");
      var thirdParagraphText = document.createTextNode("Mr Prescott would only approve skyscrapers of exceptional design. For a building of this size to be acceptable, the quality of its design is critical. He is satisfied that the proposed tower is of the highest architectural quality.");
      thirdParagraph.appendChild(thirdParagraphText);  
            document.body.appendChild(thirdParagraph);
      
var footer = document.createElement("footer");
      var footerParagraph1 = document.createElement("p");
      var footerParagraphText = document.createTextNode("Thanks for visiting our website.");
      footerParagraph1.appendChild(footerParagraphText);  
      footer.appendChild(footerParagraph1);
      
      var footerParagraph2 = document.createElement("p");
      var small = document.createElement("small");
      var footerParagraphText = document.createTextNode("Designed in 2015");
      small.appendChild(footerParagraphText);
      footerParagraph2.appendChild(small);  
      footer.appendChild(footerParagraph2);
      
      
            document.body.appendChild(footer);
      
          }, 0);

</script>

</head>
<body>
<div>

</div>
</body>
</html>

4.
function greeting(greetingText) {
return function salutation(name) {
return greetingText + " " + name;
};
}

var dayGreeting = greeting("Good morning");
var nightGreeting = greeting("Good evening");

var name = "Art";

console.log(dayGreeting(name));
console.log(nightGreeting(name));
