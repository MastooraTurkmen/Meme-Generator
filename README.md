# Meme Generator

Asalamu Alikum there,


This is my other React Project: Meme Generator. There you can click Get a new meme images and get lots of funny meme images. And also you can write on Top text and Bottom text.
Thank you So much:))))


1. By writing text the _**Top Text**_ input, you can see words on the top of the image
2. By writing text the _**Bottom Text**_ input, you can see words on the bottom of the image

![memes](https://github.com/MastooraTurkmen/Meme-Generator/assets/132576850/a8ea38df-2c2b-4a32-8462-c6937d911bbc)

![Alt text](<Screenshot 2023-10-02 104159.png>)

![meme](https://github.com/MastooraTurkmen/Meme-Generator/assets/132576850/670d50bf-4eae-4886-a84b-56d73347879b)


## Before you begin

Quick start:

````
$ npm install
$ npm run dev
$ npm start
````

````
$ pnpm install
$ pnpm run dev
$ pnpm start
````

````
$ yarn
$ yarn run dev
$ yarn start
````

Head over to https://vitejs.dev/ to learn more about using vite

-------

## Cloning the project 🪛🔨

```bash
# Clone this repository
$ git clone https://github.com/MastooraTurkmen/Meme-Generator.git

# Go inside the repository
$ cd Meme-Generator
```

-------


## Languages and Tools are used 🗣️🔧

1. **Languages** 🗣️

    + [HTML](https://github.com/topics/html)
    + [HTML5](https://github.com/topics/html5)
    + [CSS](https://github.com/topics/css)
    + [CSS3](https://github.com/topics/css3)
    + [React](https://github.com/topics/react)
    + [JavaScript](https://github.com/topics/javascript)

2. **Tools** 🔧

    + [Chrome](https://github.com/topics/chrome)
    + [Figma](https://github.com/topics/figma)
    + [VSCode](https://github.com/topics/vscode)
    + [Netlify](https://github.com/topics/netlify)


------

## Deployment 📥

1. How to deploy our project to the ***Netlify*** site?
2. I use [Netlify App](https://app.netlify.com/) for deploying my projects.
3. Go to the Netlify site and select Add a new site.
4. From there select **_Deploy with Github_**.
5. Then write your project name and select it.
6. After selecting here you can see that the project **_Review configuration for Meme-Generator_** and then select the **_Deploy Meme-Generator_** Button.
7. Now your project is Live.


-----

## React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.
Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh


## Author 👩🏻‍💻 

**Mastoora Turkmen**  

[LinkedIn](https://www.linkedin.com/in/mastoora-turkmen/) 
<br>
[Github](https://github.com/MastooraTurkmen/) 
<br>
[Twitter](https://twitter.com/MastooraJ22)


------

# Codes that are used

1. ***Index HTML***
2. ***Syle CSS***
3. ***Main JSX***
4. ***App JSX***
5. ***Components***
   + ***Header JSX***
   + ***Meme JSX***
6. ***.gitignore***
7. ***.eslintrc.cjs***
8. ***package-lock.json***
9. ***package.json***
10. ***vite.config***



## ***Index HTML***

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <link rel="icon" type="image/svg+xml" href="images/troll-face.png" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Karla:wght@400;500;700&display=swap"
      rel="stylesheet" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Meme Generator</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div id="root"></div>
    <script type="module" src="/src/main.jsx"></script>
  </body>
</html>

```

## ***Syle CSS***

```css
*,
*::before,
*::after {
  box-sizing: border-box;
}

body {
  font-family: "Karla", sans-serif;
  margin: 0;
}

main {
  padding: 36px;
}

.header {
  display: flex;
  align-items: center;
  height: 65px;
  background: linear-gradient(90deg, #672280 1.18%, #a626d3 100%);
  color: white;
  padding: 20px;
}

.header--image {
  height: 100%;
  margin-right: 6px;
}

.header--title {
  font-size: 1.25rem;
  margin-right: auto;
}

.header--project {
  font-size: 0.75rem;
  font-weight: 500;
}

.form {
  display: grid;
  grid-template: 40px 40px / 1fr 1fr;
  gap: 17px;
  margin-bottom: 17px;
}

.form--input {
  font-family: "Karla", sans-serif;
  border-radius: 5px;
  border: 1px solid #d5d4d8;
  text-indent: 5px;
}

.form--button {
  grid-column: 1 / -1;
  font-family: "Karla", sans-serif;
  border-radius: 5px;
  background: linear-gradient(90.41deg, #711f8d 1.14%, #a818da 100%);
  color: white;
  border: none;
  cursor: pointer;
}

.meme {
  position: relative;
}

.meme--image {
  max-width: 100%;
  border-radius: 3px;
}

.meme--text {
  position: absolute;
  width: 80%;
  text-align: center;
  left: 50%;
  transform: translateX(-50%);
  margin: 15px 0;
  padding: 0 5px;
  font-family: impact, sans-serif;
  font-size: 2em;
  text-transform: uppercase;
  color: white;
  letter-spacing: 1px;
  text-shadow: 2px 2px 0 #000, -2px -2px 0 #000, 2px -2px 0 #000,
    -2px 2px 0 #000, 0 2px 0 #000, 2px 0 0 #000, 0 -2px 0 #000, -2px 0 0 #000,
    2px 2px 5px #000;
}

.bottom {
  bottom: 0;
}

.top {
  top: 0;
}

@media screen and (min-width: 1000px) {
  .meme {
    text-align: center;
  }
}

```

## ***Main JSX***

```js
import React from "react";
import ReactDOM from "react-dom/client";
import App from "./App.jsx";

ReactDOM.createRoot(document.getElementById("root")).render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);

```

## ***App JSX***

```js
import React from "react";
import Header from "../components/Header";
import Meme from "../components/Meme";

export default function App() {
  return (
    <div>
      <Header />
      <Meme />
    </div>
  );
}

```

## ***Header JSX***

```js
import React from "react";

export default function Header() {
  return (
    <header className="header">
      <img src="https://i.postimg.cc/nrZtX5sg/troll-face.png" className="header--image" />
      <h2 className="header--title">Meme Generator</h2>
      <h4 className="header--project">React Course - Project 3</h4>
    </header>
  );
}

```

## ***Meme JSX***

```js
import React from "react";

export default function Meme() {
  const [meme, setMeme] = React.useState({
    topText: "",
    bottomText: "",
    randomImage: "http://i.imgflip.com/1bij.jpg",
  });

  const [allMemes, setAllMemes] = React.useState([]);

  React.useEffect(() => {
    fetch("https://api.imgflip.com/get_memes")
      .then((res) => res.json())
      .then((data) => setAllMemes(data.data.memes));
  }, []);

  function getMemeImage() {
    const randomNumber = Math.floor(Math.random() * allMemes.length);
    const url = allMemes[randomNumber].url;
    setMeme((prevMeme) => ({
      ...prevMeme,
      randomImage: url,
    }));
  }
  function handleChange(event) {
    const { name, value } = event.target;
    setMeme((prevMeme) => ({
      ...prevMeme,
      [name]: value,
    }));
  }
  return (
    <main>
      <div className="form">
        <input
          type="text"
          placeholder="Top text"
          className="form--input"
          name="topText"
          value={meme.topText}
          onChange={handleChange}
        />
        <input
          type="text"
          placeholder="Bottom text"
          className="form--input"
          name="bottomText"
          value={meme.bottomText}
          onChange={handleChange}
        />
        <button className="form--button" onClick={getMemeImage}>
          Get a new meme image 🖼
        </button>
      </div>
      <div className="meme">
        <img src={meme.randomImage} className="meme--image" />
        <h2 className="meme--text top">{meme.topText}</h2>
        <h2 className="meme--text bottom">{meme.bottomText}</h2>
      </div>
    </main>
  );
}
```

## ***.gitignore***

```bash

# Logs
logs
*.log
npm-debug.log*
yarn-debug.log*
yarn-error.log*
pnpm-debug.log*
lerna-debug.log*

node_modules
dist
dist-ssr
*.local

# Editor directories and files
.vscode/*
!.vscode/extensions.json
.idea
.DS_Store
*.suo
*.ntvs*
*.njsproj
*.sln
*.sw?

```