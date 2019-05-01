# Chemistry Website™

## [Hosted Website Link](https://dkrawciw.github.io/Chemistry-Final-Project)

# Notes:
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
  * Camel case variables (`helloWorld`, not `hello_world` or `HelloWorld`)
  * We can obviously change these, and this is just what I'm *suggesting* so all the code looks and reads consistently.

# Setup:
**To start**:  
Be sure to have the newest version of the repo (`git pull origin master`), then make sure run `npm install`.

**To lint:**  
`eslint <javascript file>.js`  
OR use the built in lint in your editor (I.E. VS Code or Atom extension)

**To run the Autoprefixer:**  
`npx postcss dev/css/*.css --use autoprefixer -d css/`

**To compile SASS:**  
`sass dev/sass:css/`

SASS only needs to be compiled when the SASS source is changed, which should range from almost never to never (once the theme is set up).


# Attempt at comprehensive documentation of the weird NPM stuff
This will still be a static site, programmed using vanilla HTML, JS + JQuery, and CSS + Bootstrap + SASS/SCSS (optionally).

You can mostly ignore anything in the `dev/` folder unless you want to write in SASS. You can ignore `.eslintrc.js` unless you want to use eslint. You can also ignore `package.json`, `package-lock.json`, and `node_modules/` unless you want to fiddle and add new packages.

Put JS for *all* html pages in `js/app.js`, and for js for a single page, place it in inline JS or create a new file in `js/` and embed it in the html.  
Same with vanilla CSS, only with `css/app.css` and `css/` instead. However, try to avoid writing plain CSS, and instead use Bootstrap wherever possible. You can do most anything with Bootstrap, and don't be afraid to look at the [bootstrap docs](https://getbootstrap.com/docs/4.3/getting-started/introduction/). If you need something like a new color, put it in `dev/sass/bootstrap/_variables.scss` if you know how to or have Alex do it.