# Rick & Morty 

<div style="display: flex; justify-content: center;">
<img src="https://i.ibb.co/6ZYK1ys/logo.jpg" width="200px" height="200px"/>
</div>


## How to run :running_man:

* **Server**
    1. Go to the Server repo and run `npm install` to install dependencies.
    3. install redis and run command `redis-server` to have access to redis database.
    2. run command `npm run start`. open `http://localhost:4000/graphql` to see the GraphQl playground.
    
* **App**
    1. Go to the front repo and run `yarn` to install dependencies.
    2. run command `yarn start` then open browser and see `http://localhost:3000`.

I also make dockerie th front project. for this purpose i create a `Dockerfile` and `docker-compose.dev.yml` file.



## What was in my mind :brain:

I do try to avoid using additional package and just use the essential packages to keep the project minimal. In the front part I just used **React**, **sass**, **Apollo client**, **eslint** , **prettier**, **husky** and **commitlint**. Below I will explain the uses and reasons for choosing these tools for front part .

### Front End
 
* **React** : The core and framework :sweat_smile:

* **Sass**: Using sass makes coding styles more enjoyable with providing the variables and allow to wring function in css. I write some basic class for display, positions , and breakpoints in `src/assets/design` and import it in the `index.jsx` in order to available in the all files (components and pages ).

* **Apollo client** : For request graphQL API in the front.

* **eslint with prettier** : These tools have been used for keep coding style clean .

* **husky**: This great tool to do pipeline in deve mode before pushing the codes. I config husky with commitlint .

* **commitlint** : It is interesting package for checking the commits before push to have goode commit convention.

### Back End

I have implemented the backend with **node.js** and **typescript** (ts-node), **graphql-yoga**, **code-gen** ,**mongodb**, **redis**, **tslint** with **prettier**, **husky** with **commitlint** and **nodemone**.

* **GraphQL-Yogo**: It is amzaing for using graphql in server. I preferred **GraphGL-Yogo** over **Apollo Server** because this project was samll and GraphQL Yoga only has a fraction of the dependencies of Apollo Server, and in general is much smaller. Also GraphQL Yoga's APIs are designed for code-splitting and thus have no side effects, where Apollo server specifies that is has side effects and thus, cannot be code splitted.

* **Code-gen**: It is a great tools for generating types of typescript based on the schema file. As you know the schema file determine the input and types in graphql that is pretty like the types in typescript but it's different! if you want convert the schema types to the typescript types it is cumbersome. Here that Code-gen comes to produce types base on schema file. `codegen.yml` is the confige file.

* **mongodb**: The detabase for saving users (use cloud mongodb atlas ).

* **redis**: Favourite cache database for caching characters cards.

* **nodemone**: Using in order to hot reloading.

* **tslint with prettier**: Like eslint with prettier in the front.
