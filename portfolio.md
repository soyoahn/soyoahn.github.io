---
title: Portfolio
layout: default
---
<script>
//SCROLL TO TOP

var mybutton = document.getElementById("buttonTop");

function scrollFunction() {
  if (document.body.scrollTop > 1000 || document.documentElement.scrollTop > 1000) {
    mybutton.style.display = "block";
  } else {
    mybutton.style.display = "none";
  }
}

function topFunction() {
  document.body.scrollTop = 0;
  document.documentElement.scrollTop = 0;
}
</script>

{%- include casestudies.html -%}

{%- include writingsamples.html -%}
<button onclick="topFunction()" id="buttonTop" title="Go to top">Top</button>
