## Install Ghost

You need to install Ghost locally in order to test your changes. You can install Ghost by following the steps below.

1. Install Ghost-CLI

```
npm install ghost-cli@latest -g
```

2. Install Ghost

Create an empty directory and run:

```
ghost install local
```

3. Run Ghost

Start Ghost if it's not already running:

```
ghost start
```

4. Access your blog

Access the blog at `http://localhost:2368` and the admin interface at `http://localhost:2368/ghost`.

> For more information about installing Ghost, check out their [documentation here](https://ghost.org/docs/install/local/).

## 🔠 Setup custom google fonts

1. Go to [fonts.google.com](https://fonts.google.com/) and choose a font.
2. Choose __Embed__ and copy the `<link>` code.
3. Go to __Code injection__.  
4. Add this to __Blog Header__:  
````html
<link href="https://fonts.googleapis.com/css2?family=Mukta&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Crimson+Text&display=swap" rel="stylesheet">
<style>
  :root {
    --font-primary: 'Mukta', sans-serif;
    --font-secondary: 'Crimson Text', serif;
  }
</style>
````

## ⚙️ Development

Install [Grunt](https://gruntjs.com/getting-started/):
````bash
npm install -g grunt-cli
````
Install Grunt dependencies:
````bash
npm install
````
Note: If your install gets stuck, try this method:
````bash
npm install -g npm@6
````

Build Grunt project:
````bash
grunt build
````
The compress Grunt task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.
````bash
grunt compress
````

## 💻 Testing

Before opening a PR, validate the theme and make sure it works properly. You can validate the theme at https://gscan.ghost.org/. Upload a zip to check for errors, deprecations and other compatibility issues.

## ⚖️ Copyright & License

Copyright (C) 2015-2022 Peter Amende - Released under the [MIT License](https://github.com/zutrinken/attila/blob/master/LICENSE).
# attila-theme
