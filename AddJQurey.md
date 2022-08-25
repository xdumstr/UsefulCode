## Run this code in console
```js
(function() {
  // Load the script
  const script = document.createElement("script");
  script.src = 'https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js';
  script.type = 'text/javascript';
  script.addEventListener('load', () => {
    console.log(`jQuery ${$.fn.jquery} has been loaded successfully!`);
    // use jQuery below
  });
  document.head.appendChild(script);
})();
```

## You can use jqurey functions in console

[W3 Schools](https://www.w3schools.com/jquery/default.asp)
