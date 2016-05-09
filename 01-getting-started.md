# Getting Started

### Overview 
In this module you will:
- Learn to access the console section of your browser
- Create a basic HTML file 
- Add inline JavaScript to HTML file
- Using the HTML script tag to host the JavaScript for the HTML document
- Create a JavaScript file 
- Run some JavaScript code from an external JavaScript file
- Learn to comment JavaScript code

### Accessing the console from your browser
In this section we will be using the Google Chrome web browser to run a simple command in the console area.
- Open Google Chrome webbrowser
- Press ctrl+shift+i or right-click anywhere on the screen and press **inspect**
- Click on the Console tab on the top 
- On the bottom there should be a window called **Console**, in the console window type **console.log("Hello, World!")** and press enter 

### So what just happened
The console window is used to interact with the browser's JavaScript Engine in this case because we are using Google Chrome we have access to the JavaScript V8 engine to run simple JavaScript commands. In our example we instructed the console to log the statement **Hello, World!** to the console.

### Executing JavaScript from the browser
In this section we are going to create an html file and add some inline JavaScript to your browser and then refactor the file so that the JavaScript will be in it's own seperate file.

#### index.html
        <!doctype html>
        <html>
          <head>
            <meta charset="utf-8">
            <title>Hello World</title>
          </head>
          
          <body>
          
          <script src="main.js"></script>
          </body>
        </html>

#### main.js
        //Instruct Console to log statement Hello, World!
        console.log("Hello, World!");

### Conclusion
In this module we created an html document and added a script tag just before the closing body tag.
