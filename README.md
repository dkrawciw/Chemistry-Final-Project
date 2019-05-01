# Chemistry Website™

Setup:
Simply run `npm install`

To run the Autoprefixer:  
`npx postcss dev/sass/*.css --use autoprefixer -d css/`

To compile SASS:  
`sass dev/sass:css/`

Run the autoprefixer before compiling SASS  
SASS only needs to be compiled when the SASS source is changed, which should range from almost never to never (once the theme is set up).
