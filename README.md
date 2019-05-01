# Chemistry Website™

Notes:
* I've included a .eslintrc.js that I use, but since I don't speak for the whole group we can talk about it next class
  * You are obviously not obligated to (or expected to) use ESLint, but since I do and I was installing basic modules I installed it anyway.
* Even if you aren't using ESLint, we should probably code in a consistent style, which we can talk about next class, but basic style that I would suggest would be:
  * 2 spaces for a tab
  * Single quotes for strings (unless double quotes are nessessary, I.E. apostrophes in string)
  * Spaces after if and function declarations
    * `for (i = 0...` and `function whatever (arg1)...` instead of `for(i = 0...`
  * K&R style brackets
    * `function whatever () {` instead of 
    * `function whatever ()`  
      `{`
  * We can obviously change these, and this is just what I'm *suggesting* so all the code looks and reads consistently.

Setup:  
Simply run `npm install`

To lint:
`eslint <javascript file>.js`  
OR use the built in lint in your editor (I.E. VS Code or Atom exension)

To run the Autoprefixer:  
`npx postcss dev/sass/*.css --use autoprefixer -d css/`

To compile SASS:  
`sass dev/sass:css/`

Run the autoprefixer before compiling SASS  
SASS only needs to be compiled when the SASS source is changed, which should range from almost never to never (once the theme is set up).
