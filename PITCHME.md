# AWS Lambda

## Key notes

---

## What

---

## What is Lambda

- Serverless from Amazon |
- Lets you run the code  in a "stateless" style |
- Amazon manages the infrastructure on your behalf |
- Code is written in .NET Core, NodeJs, Java, Python or Go |

In the most basic form it is just a single class (C#) or a single function (NodeJs). It can also be the whole application with external libraries as long as it fits into constraints
that serves as an entry point that runs in response to certain events. 

---

## What is alternative

---

## What is pricing model

AWS Lambda is metered in increments of 100 milliseconds

---

## Who

---

## Who is using lambda

---

## How

---

## How it looks

---

## How it works

---

## How to deploy

---

## How to troubleshoot

---

## But

---

### Cons

- There is no SLA
- What to do when AWS Lambda is down

---

## External references

- https://docs.aws.amazon.com/lambda/latest/dg/current-supported-versions.html
- 

---


@title[JavaScript Block]

<p><span class="slide-title">JavaScript Block</span></p>

```javascript
// Include http module.
var http = require("http");

// Create the server. Function passed as parameter
// is called on every request made.
http.createServer(function (request, response) {
  // Attach listener on end event.  This event is
  // called when client sent, awaiting response.
  request.on("end", function () {
    // Write headers to the response.
    // HTTP 200 status, Content-Type text/plain.
    response.writeHead(200, {
      'Content-Type': 'text/plain'
    });
    // Send data and end response.
    response.end('Hello HTTP!');
  });

// Listen on the 8080 port.
}).listen(8080);
```

@[1,2](You can present code inlined within your slide markdown too.)
@[9-17](Displayed using code-syntax highlighting just like your IDE.)
@[19-20](Again, all of this without ever leaving your slideshow.)

---

## Template Help

- [Code Presenting](https://github.com/gitpitch/gitpitch/wiki/Code-Presenting)
  + [Repo Source](https://github.com/gitpitch/gitpitch/wiki/Code-Delimiter-Slides), [Static Blocks](https://github.com/gitpitch/gitpitch/wiki/Code-Slides), [GIST](https://github.com/gitpitch/gitpitch/wiki/GIST-Slides) 
- [Custom CSS Styling](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Custom-CSS)
- [Slideshow Background Image](https://github.com/gitpitch/gitpitch/wiki/Background-Setting)
- [Slide-specific Background Images](https://github.com/gitpitch/gitpitch/wiki/Image-Slides#background)
- [Custom Logo](https://github.com/gitpitch/gitpitch/wiki/Logo-Setting) [TOC](https://github.com/gitpitch/gitpitch/wiki/Table-of-Contents) [Footnotes](https://github.com/gitpitch/gitpitch/wiki/Footnote-Setting)

---