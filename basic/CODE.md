# Code

## Draft 01: Basic JS and DOM

```html
<html>
  <body>
    <div id="app"></div>
    <script src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
    <script type="text/javascript">
      const app = document.getElementById('app');
      const header = document.createElement('h1');
      const text = 'Example Product';
      const headerContent = document.createTextNode(text);
      header.appendChild(headerContent);
      app.appendChild(header);
    </script>
  </body>
</html>
```

## Draft 02: Try to write HTML on JS

```html
<html>
  <body>
    <div id="app"></div>
    <script src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
    <script type="text/javascript">
      const app = document.getElementById('app');
      const root = ReactDOM.createRoot(app);
      root.render(<h1>Wow! That's the React DOM.</h1>);
    </script>
  </body>
</html>
```

## Draft 03: Writing HTML with JS using Babel to make it complete

```html
<html>
  <body>
    <div id="app"></div>
    <script src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <script type="text/jsx">
      const domNode = document.getElementById('app');
      const root = ReactDOM.createRoot(domNode);
      root.render(<h1>Wow! That's the React DOM.</h1>);
    </script>
  </body>
</html>
```
