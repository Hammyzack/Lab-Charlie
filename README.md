# Dev Lab CHARLIE/486 Story Card 

## User Story (Story Points = med👕) 

**As a** user of your hello-node app

**I want** <del>to use this app online, _on the web_</del> to interact with the app: type and respond. 

**So That** my app does something a little more

## Comments/Discussion
- use node.js + express.js + angular.js

## Resources
- 

## Test/Acceptance Criteria/Rubric (how do you know when you are done) 

- [x] navigate to a URL: _______ (heroku): 0 | 5 | 10
- [x] app has a  link back to ghyt repo w/target: 0 | 5 | 10
- [x] file directory and naming, ghyt link to heroku: 0 | 5 | 10 
- [x] readme: explain some about angular...how user types in input and where that data goes from there, use code hightlight syntax in markdown: 0 | 5 | 10 
- [x] code quality: logical, readable, functional: functional = loads user json data, changes input data; updates a file on the server0 | 5 | 10  

## How to use Angular

The first thing the user will see when they open up the main page is the `user.json` message that says
"and hi there, tom tom". This is being displayed by the code below!

```
app.get('/user', function (req, res) {

    res.sendFile('/user.json', { root: __dirname });

});
```

The user then will see the **html** that was created that will display **My-Angular** with my name. It will also ask them if they are lost or confused. Then it continues by giving them `URL Links` to help them get to where they need to be. Below is the code that displays the main page for the html.

```
<div class="row">
            <div class="col-md-8 offset-md-2">
                <h1 id="page-title">My-Angular</h1>
                <input ng-model="user.name">
                <h3 id="user-greeting">Welcome I'm Hammy, {{ user.name }}</h3>
                <p id="user-car">Lost or confused{{ user.car }}? Click on the links above!!</p>
            </div>
```
