<h1 style="margin-left:0 auto">My own take on <span style="color:green">NodeJS</span></h1>

**`Please note that this is my personal overview on node ,this maybe not 100% correct`**

Wouldn't it be awesome if you only had to know one programming language for building a full stack application? Ryan Dahl put this thought into action and created Node.js. Node.js is a server side framework that is built upon Chrome's powerful V8 JavaScript engine. Though originally written in C++, it uses JavaScript to be used in applications.

See, problem solved. One language to rule them all. But this also brings you down to the fact that now your whole application is using the same language. That means you must have a sound knowledge of that language.


*If you write front end code, it shouldn’t be news that you could easily write web apps with NodeJs since both rely heavily on JavaScript.*

It’s very important to understand that Node isn’t a silver bullet, it’s not always the best solution for every project. Anybody can start up a server in Node, but it takes a deeper understanding of the language to write web apps that scale.

Recently, I’ve been having a lot of fun with Node and I think I’ve learned enough to share, get feedback and learn more. Generally to cement my knowledge.

<h1>Before Node.js.</h1>

Web applications were written in a client/server model where the client would demand resources from the server and the server would respond with the resources. The server only responded when the client requested and would close the connection after each response.

This pattern is efficient because every request to the server takes time and resources(memory, CPU etc). So, it’s wiser to close a connection after serving the requested asset so the server could respond to other requests too.

So how do servers like these respond to millions of requests coming in at the same time? If you asked this question, you understand that it wouldn’t be nice if requests to servers would be delayed till all other requests were responded to.

Imagine visiting Facebook and you were told to wait for 5 minutes, for thousands of people requesting before you. There has to be a way to run thousands or at least hundred of requests at once. Good news!!. There’s a thing as Threads.

Threads are a way for systems to run multiple operations concurrently. So every request would open a new thread, every thread had all it required to run the same code to completion.

If it sounds strange?. Let’s use this analogy.

<h3>Strong Foundations of NodeJS</h1>

**`Modules`** : *A reusable block of code whose existence does not accidentally imapct other code*(it was not present in vanilla JS)




`
Imagine a restaurant with just one person serving food.When the demand for food increases, things would crazily go wrong. People would have to wait till all preceding orders were delivered A way to solve this problem would be to employ more people to serve food right? This way, more customers would be served at once.
`


Each thread is a new employee and the browsers, well, hungry people. I’m sure you can get the point now.

But this system has a downside.**It would get to a point where there’s a lot of requests and starting up new threads would consume a whole lot of memory and system resources.**







<img src="https://images.idgesg.net/images/article/2018/04/iwan_05-100755063-orig.jpg"
     alt="intro"
     style=" margin:0 auto;eidth:300px;height:200px" />
