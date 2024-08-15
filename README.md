<h1>TailwindCSS Install Process :wave:</h1>

## Welcome all :point_right:
Here you will learn all the topics of the TailwindCSS and hopefully you will be mastered on the TailwindCSS. I will be happy to teach you all you need to know about TailwindCSS. So let's dive in. :wink:

First you need to install on your machine `NodeJS`

Second make a Directory then open the VSCode Teminal Or GitBase Any Terminal.

Make a `index.html` File

Make `package.json` file bellow command

```sh
npm init
```
Then Just Enter

Then open `package.json` and add this.

```sh
"keywords": [],
```

Install TailwindCSS with `postcss` and `autoprefixer`

```sh
npm install -D tailwindcss postcss autoprefixer
```

Now lets create both `tailwind.config.js` and `postcss.config.js`

```sh
npx tailwindcss init --postcss
```

After that lets create `tailwind.css` a genarel CSS file and place there these directives

```sh
@tailwind base;
@tailwind components;
@tailwind utilities;
```

and then lets modify the `tailwind.config.js` file with the following code (remember to edit it according to your project's source files and directories)

```sh
content: ["./src/**/*.{html,js}"],
```

Finally, lets write a script to watch the css file (remember to edit it according to your project's source files and directories)

```sh
npx tailwindcss -i ./tailwind.css -o ./src/output.css
```

Open `package.json` `script` section add this

```sh
"watch": "npx tailwindcss -i ./tailwind.css -o ./src/style.css --watch"
```

`index.html` file linked css file

```sh
<link rel="stylesheet" href="src/style.css" />
```


Finally run the watch command

```sh
npm run watch
```





