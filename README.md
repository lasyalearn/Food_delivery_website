# 🥟🥡Food_delivery_website🍜🥞
## learn with me 😀
React is used for creating single web pages.....
React makes use of JSX instead of javascript....
the differences betweeen the two are:-
1. change in reserved words( JAvascript uses class...While JSX uses className)
before planning ur website always segregate between reusable components and screens(planning is key)
### ---------------------------------------------------------------------------------------------------------
## intial setup-------(if ur building from scratch😁)
npx create-react-app food_app ---> is used to create the react app ------> food_app folder is created with some pre-written files
to run the react app you need to enter the food_app folder --------> cd food_app ------> then ----->npm start
Now u will the default react web site
![image](https://github.com/user-attachments/assets/4b157459-4052-461a-9368-83d32c2d78dc)
which will run on localhost:3000
now intall when we code in app function in app js 
and when we install something seperately  it should be added in the dependencies
but  if place the <link href="https://cdn.jsdelivr.net/npm/bootstrap-dark-5@1.1.3/dist/css/bootstrap-night.min.css" rel="stylesheet"> on top of the head the no need to install bootstrap and and it in dependecies
the  dependecire\es are present in package.json file 
also the fs-1 class is part of bootstrap (ig)😅----> it is used to increase the font size
font-family: 'NHaasGroteskDSPro-65Md' !important; ----------> is added to index.css
important!---> it seems that index.css will effect the whole project it seems
for the above to tak eeffect we should add <link href="https://db.onlinewebfonts.com/c/f21923cb0f60b46d41a66875255790b3?family=NHaasGroteskDSPro-65Md" rel="stylesheet" type="text/css" /> in index.html just before index.html
### ---------------------------------------------------------------------------------------------------------
## Compoents for the react page
components are something which are reuseble on every screen
Let's learn how to create various components in react
create a new folder called components in src and each which we will create file in components will be a component of the react web page 
All the component file should start with a capital letter.
1. component we will create is Navbar.js (inside if tpye rfc ---> we will get the default code ).Here we used some bootstrap default code. (class is wrong so change all the class to the className and routing needed be used)(/ --> home page default )(so intial it mean ur routing back to the same home page  which is == to reloading the page)                                            ->navbar-expand-lg------>This class makes the navbar responsive. It specifies that the navbar should be expanded (i.e., horizontal) on large screens (lg and up), but collapse into a vertical menu on smaller screens.                       
           ->nav-dark------>This class will making the writing in the navbar will be dark                                    
           ->bg-success---->This class will give the background to the navbar (which defaultly will be green  which is set by bootstrap)                                                                                                               All the css in bootstrap are predefined class (liked mentioned before fs-1----> increases the size)( fst-italic)              And one more thing I have noticed is that if u type the class name wrong also the error won't show up only that styling will not come( font related for now)          
2. we have also create the footer component
3. 

### ---------------------------------------------------------------------------------------------------------
## 📕Notes and explanations
1.it seems in react function we can't have multiple divs ---> to help with this we need to enclose in the multiple div in a empty parent tag<></>  or a div(a div can have multiple div tages inside of it)
2.after creating a component in the components folder it won't reflect in main app web page unless we need import th file and use it as a tag

### ---------------------------------------------------------------------------------------------------------
## screens are the different web pages(like home page, order page  and so on...)
1. Home page(here also we type rfc to get the default code page where we called the navbar and the footer component)(how to the handle the anchor tag)(the anchortage is used to go to the next page)
2.App.js the default file u get when u create the react app will have the (all the routes to diferent screens)
3.Login page
### ---------------------------------------------------------------------------------------------------------
## 📕Notes and explanations
### ---------------------------------------------------------------------------------------------------------

### ---------------------------------------------------------------------------------------------------------
## routers in react (used to navigate from one react page to another)
To make us of router we need to install react router dom ------> npm i react-router-dom
check in the package.json file whether it is added in the dependencies
as mentioned before
 we use react router to replace all of anchor tags
 to use the above first we need to import ----------> import {BrowserRouter as Router, Switch, Route, Link} from "react-router-dom"; in the home page 
1.  creaated a route for the home page
2.  login page
### ---------------------------------------------------------------------------------------------------------
## 📕Notes and explanations
### ---------------------------------------------------------------------------------------------------------
##Extra

1.if ur getting this warning 
ans-->One of your dependencies, babel-preset-react-app, is importing the
"@babel/plugin-proposal-private-property-in-object" package without
declaring it in its dependencies. This is currently working because
"@babel/plugin-proposal-private-property-in-object" is already in your
node_modules folder for unrelated reasons, but it may break at any time.

babel-preset-react-app is part of the create-react-app project, which
is not maintianed anymore. It is thus unlikely that this bug will
ever be fixed. Add "@babel/plugin-proposal-private-property-in-object" to
your devDependencies to work around this error. This will make this message
go away.
install 
npm install --save-dev @babel/plugin-proposal-private-property-in-object


2.There is an another warning   Line 5:1:  Unexpected default export of anonymous function  import/no-anonymous-default-export     
ans--> the problem was that (when u pressed rfc and the default code comes)(it has function (export default function <function name()>) sometime back the function name got erased by mistake and hence the error came to be)
I will push the project at the end( for now i will edit the readme file only everyday)
learning from youtube channel:- end to end 
