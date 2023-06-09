# Rick & Morty 

<div style="display: flex; justify-content: center;">
<img src="https://i.ibb.co/6ZYK1ys/logo.jpg" width="200px" height="200px"/>
</div>


## What was in my mind :brain:

I do try to avoid using additional package and just use the essential packages to keep the project minimal. In the front part I just used **React**, **sass**, **Apollo client**, **eslint** , **prettier**, **husky** and **commitlint**. Below I will explain the uses and reasons for choosing these tools for front part .

### Front End
 
* **React** : the core and framework :sweat_smile:

* **Sass**: Using sass makes coding styles more enjoyable with providing the variables and allow to wring function in css. I write some basic class for display, positions , and breakpoints in `src/assets/design` and import it in the `index.jsx` in order to available in the all files (components and pages ).

* **Apollo client** : for request graphQL API.

* **eslint with prettier** : These tools have been used for keep coding style clean .

* **husky**: this great tool to do pipeline in deve mode before pushing the codes. I config husky with commitlint .

* **commitlint** : it is interesting package for checking the commits before push to have goode commit convention.

### Back End

I have implemented the backend with **node.js** and **typescript** (ts-node), **graphql-yoga**, **code-gen** ,**mongodb**, **redis**, **tslint** with **prettier**, **husky** and **commitlint**
