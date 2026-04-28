1. The bug was that the line let num1 = document.getElementById("num1").value; does not return an integer, but rather a string. Thus concatenation happens instead of proper addition.
