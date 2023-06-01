Step 01: generate package.json file
npm init -y

step 02: install development environment

npm install -D tailwindcss postcss autoprefixer vite

step 03: generate tailwind.config.js and postcss.config.js

npm tailwindcss init -p 


step 04: set run environment using vite
package.json

 "scripts": {
    "start": "vite"
  },

step 05: load tailwincss in your css file
style.css

@tailwind base;
@tailwind components;
@tailwind utilities;

step 06: use tailwindcss in whole project

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ['*'],
  theme: {
    extend: {},
  },
  plugins: [],
}

step 07: link style.css file in your html file
index.html
 <link rel="stylesheet" href="css/tailwindcss.css">

step 08 : run your project
npm run start 
































