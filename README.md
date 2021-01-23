# tailwindtemplatelighthouse
Portfolio
TAILWIND PROCESS GUIDE FROM COMMAND LINE

mkdir NEWSITE

cd NEWSITE

git clone 

CD tailwindfamily
	
		if no GITCLONE AVAILABLE MOVE TO PROCESSS 2

Process 2:

npm install tailwindcss@latest postcss@latest autoprefixer@latest

TOUCH BUILD

TOUCH DIST

TOUCH JS

TOUCH JSINC

TOUCH  MEDIA

TOUCH SRC

TOUCH postcss.config.js

TOUCH tailwind.config.js

VIM postcss.config.js
// make sure looks like this //
module.exports = {
    plugins: {
      tailwindcss: {},
      autoprefixer: {},
    }
  }


VIM tailwind.config.js
// make sure looks like this //
module.exports = {
  purge: [
    'src/**/*.html',
    'src/**/*.vue',
    'src/**/*.jsx',
  ],
  darkMode: false, // or 'media' or 'class'
  theme: {
    extend: {},
  },
  variants: {
    extend: {},
  },
  plugins: [],
}

//most important command//

build css file with changes added to tailwind.css in src file

npx tailwindcss-cli@latest build ./src/tailwind.css -o ./dist/tailwind.css***********








Build tailwind for production with min css

NODE_ENV=production npx tailwindcss-cli@latest build ./src/tailwind.css -o ./dist/tailwind.css



<div class="flex">
  <div class="flex-1 ...">
    <!-- Will grow and shrink as needed without taking initial size into account -->
  </div>
  <div class="flex-1 ...">
    <!-- Will grow and shrink as needed without taking initial size into account -->
  </div>
  <div class="flex-1 ...">
    <!-- Will grow and shrink as needed without taking initial size into account -->
  </div>
</div>

    <div class="fixednav">
    <nav class="nav flex 	 flex-wrap items-center justify-between px-4">
        <div class="flex flex-no-shrink items-center mr-6 py-3 text-grey-darkest justify-self-center">
          	
          <a href="index.html">
            <!-- Company Name -->
          <span class=" font-semibold tracking-tight">US Family Marketing</span>
        </div>
    </a>



