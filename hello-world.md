### Hello World
React is a javascript library, so before start developing in react, first we have to download [node](https://nodejs.org/en/). Download any stable version of node, npm (Node package manager) will be available in same downloaded file. NPM helps you to download packages and open source libraries to make your react applications more cool. once you have downloaded and installed node JS you can verify installation using. 

```properties
> node -v
``` 
It will also install `npm` automatically along with `nodeJs`

All setup, let's move to create simple hello world react app.

Go to the directory where you want to create react application, open powershell and type following commands. Hold a cup of tea because this process will take some time to download required packages for react `hello-world` application.

```properties
npx create-react-app hello-world
cd hello-world
npm start
``` 

This will start your application `http://localhost:3000/`
![npm-start](https://github.com/hafizusman530/time-to-react/blob/master/npm-start.png)

If you want to serve react application on `nginx`, just download [nginx](https://www.nginx.com). `Nginx` is web server that is best to serve static web contents. Let's build our react application into production ready package and deploy on nginx.

```properties
npm run build
```

This command wil create a build folder packaged all our react application content, copy build folder (rename it if you want) and paste into `http` folder of your nginx server. If your nginx is running on port `80` you can then access react application deployed on nginx using following url.

`http://localhost:80/build`
