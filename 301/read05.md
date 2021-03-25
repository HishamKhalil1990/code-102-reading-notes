# Node.js For Beginners. Deploy Your Blog to Heroku
### Node.js is an open source, cross-platform runtime environment, which allows you to build server-side and networking applications. using javascript to write on Node.js, it can run on any platform. it acts like a server.
### Heroku is a cloud platform as a service, It allows you to deploy your web server, for using you need to:
- create account
- install Heroku
### to create a server:
1. Create your project directory. And then create the server.js using the following:
    - ![ex](https://i.ibb.co/7j8PxyW/2.jpg)
    - The first one is for giving the key to Node's HTTP functionality. The second one is for possibility to interact with the file system. The third one allows to handle file paths. The last one allowsto determine a file's MIME-type.
2. Create the package.json file as the following:
    - ![ex](https://i.ibb.co/mRFvdr4/3.jpg)
    - it includes "name", "version", "description", and "dependencies"
3. create send404() function as the following:
    - ![ex](https://i.ibb.co/d6Ny0yK/4.jpg)
4. define sendPage() function as the following:
    - ![ex](https://i.ibb.co/N1Q8zCX/5.jpg)
5. define handle responses as the following:
    - ![ex](https://i.ibb.co/qDd5RYb/6.jpg)
6. create the HTTP server as the following:
    - ![ex](https://i.ibb.co/SXvdPNM/7.jpg)
7. create the `index.html` file. for example:
    - ![ex](https://i.ibb.co/ZLwXyqK/8.jpg)