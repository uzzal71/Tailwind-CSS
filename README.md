# Tailwind-CSS
## 01 Introduction | Tailwind CSS
## 02 Tailwind Installation 
Tailwind Installation & Editor Setup
Three type Instllation process in tailwind css
1. Install from CDN
2. Install as PostCSS Plugin
3. Install Tailwind CLI

Here, Tailwind CSS Install With CLI

- npm init -y
- npm i -D tailwindcss
- VS Code Install -> Tailwind CSS IntelliSense
- npx tailwindcss init [This command create tailwind.config.js]

```
module.exports = {
  purge: [],
  darkMode: false, // or 'media' or 'class'
  theme: {
    extend: {},
  },
  variants: {
    extend: {},
  },
  plugins: [],
};

```
- Then, project folder create two folder are called - output, src
- Create src/tailwind.css file [This file name hold any name]
- Open src/tailwind.css and write them

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
Create .vscode/settings.json file

Open .vscode/settings.json file
```
{
	"css.validate": false,
	"tailwinCSS.emmetCompletions": true
}
```

Create a build script & open package.json file

```
"scripts": {
    "build": "tailwindcss -i ./src/tailwind.css -o ./output/tailwind.css -w"
}
```

Run Build Command In Your Terminal
```
npm run build
```

When Run This Command output/tailwind.css file generated. This tailwind.css file linkup index.html file.
```
<link rel="stylesheet" href="./output/tailwind.css" />
```

## 03 Utility-First Approach | Tailwind CSS 
Tailwind Utility-First Design Approach | tailwindcss

## 04 Responsive variants - Tailwind Breakpoints | Tailwind CSS 