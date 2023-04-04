<div id="header">Header</div>
#header {
  background-color: #f1f1f1; /* Grey background */
  padding: 50px 10px; /* Some padding */
  color: black;
  text-align: center; /* Centered text */
  font-size: 90px; /* Big font size */
  font-weight: bold;
  position: fixed; /* Fixed position - sit on top of the page */
  top: 0;
  width: 100%; /* Full width */
  transition: 0.2s; /* Add a transition effect (when scrolling - and font size is decreased) */
}

// When the user scrolls down 50px from the top of the document, resize the header's font size
window.onscroll = function() {scrollFunction()};

function scrollFunction() {
  if (document.body.scrollTop > 50 || document.documentElement.scrollTop > 50) {
    document.getElementById("header").style.fontSize = "30px";
  } else {
    document.getElementById("header").style.fontSize = "90px";
  }
}
