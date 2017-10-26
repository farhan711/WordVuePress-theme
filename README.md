![image](https://d2jq2hx2dbkw6t.cloudfront.net/605/vuejs-wordpress.jpg)


# WordVuePress Theme 
This Theme will Grab all the VueJs components to your Wordpress theme.
Learn Vue inside WordPress, or to create your own theme.
It also includes an example component or you can create your own component. 
In this theme Webpack is used to compile the assets. 
``` webpack-dev-server ``` and ``` HMR ``` to avoid page reload on asset change. 
Also added ``` browserSync ``` for auto reloading on PHP file change. 

Please Note : There are packages you would probably want to use such as axios, vuex, etc. I would leave them to you to install. 

# Steps:

Clone the theme, run ```npm install``` and  Booyah! Start playing. 

But make sure to modify the ``` BrowserSync ``` proxy  link inside the ``` webpack.config.js ``` 

## Note 
``` webpack-dev-server ``` serves assets from memory, which means that on development mode.
Also we would have to include asset files from 
``` http://localhost:8080/[name].css ``` and ``` http://localhost:8080/[name].js ```. 
When you switch to production you remove these links and remove the comment tags from the asset links to the current directory. Also
I added comments in the functions.php file to make it more clear. 

# Keep in mind that you need to run ``` npm run dev ```, otherwise you would get 404 on the development asset links.

## Commands to be used in installing and setup this theme
1. ``` npm run build ``` Will compile and minify assets for produciton.
2. ``` npm run build:dev ``` Will compile assets. 
3. ``` npm run dev ``` Will compile and start webpck-dev-server and browserSync. 

(NOTE: Also make your you install all other general dependencies to run the nodeJS and Server.)

## Also Vue devtools to develop 
Click to download devtools [here](https://github.com/vuejs/vue-devtools#vue-devtools)
