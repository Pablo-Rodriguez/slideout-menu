# slideout-menu

Polymer web component for the slideout.js library

##Install

```
$ bower install --save slideout-menu
```

## Usage

``` html
<!doctype html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
  <title>slideout-menu</title>
  <!-- We import polymer  -->
  <link rel="import" href="bower_components/polymer/polymer.html">
  <!-- We import slideout-menu  -->
  <link rel="import" href="bower_components/slideout-menu/slideout-menu.html">
</head>
<body>
  
  <slideout-menu>
    
    <!-- We create a container for the menu (the menu class is needed)  -->
    <nav class="menu">
      <header>
        <h2>Menu</h2>
      </header>
    </nav>

    <!-- We create a container for the main content (the panel class is needed)  -->
    <main class="panel">
      <header>
        <button class="toggle-menu">MENU</button>
        <h2>Main content</h2>
      </header>
    </main>
  
  </slideout-menu>
  
  <script>
    var menu = document.querySelector('slideout-menu');
    document.querySelector('.toggle-button').addEventListener('click', function () {
      menu.toggle();
    });
  </script>

</body>
</html>
```

## API

Read the slideout.js documentation for the api documentation. You can access the same methods both in the library and the web component. If you realize a slideout.js method is not implemented you can use the .slideout property of slideout-menu which is and instance of Slideout.
