[README.MD](README.md)   
[Server Architecture](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data)

**Form Data**  
_Where does the data go, and how do we handle it when it gets there?_  

**Client/server architecture**  
- he web uses a client/server architecture that can be summarized as follows. a client (usually a web browser) sends a request to a server (most of the time a web server like Apache, Nginx, IIS, Tomcat, etc.), using the HTTP protocol. The server answers the request using the same protocol.  
- An HTML form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server. This enables the user to provide information to be delivered in the HTTP request.  
- Using the <form> element directs the data as its being sent. Two most important attributes  are _action_ and _method_ .  
- _Action_ defines where the data gets sent. Value must me relative or absolute URL.  
- The _name_ and _values_ of the non-file form controls are sent to the server as name=value pairs joined with ampersands. The action value should be a file on the server that can handle the incoming data, including ensuring server-side validation.  
- The _method_ attribute defines how data is sent. The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted via a number of different methods, the most common being the **GET** method and the **POST** method.  
- The **GET** method is the method used by the browser to ask the server to send back a given resource: "Hey server, I want to get this resource". The browser sends an empty body. Because the body is empty, if a form is sent using this method the data sent to the server is appended to the URL.  (this was just an example).  
- The **POST** method is a little different. It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request: "Hey server, take a look at this data and send me back an appropriate result." If a form is sent using this method, the data is appended to the body of the HTTP request.  
**Viewing HTTP Request**  
- HTTP requests are never displayed to the user (if you want to see them, you need to use tools such as the Firefox Network Monitor or the Chrome Developer Tools). As an example, your form data will be shown as follows in the Chrome Network tab. After submitting the form.  
    - Open Dev tool  
    - Select "Network"  
    - Select "All"  
    - Select "xxx.com" in the "Name" tab  
    - Select "Headers"  
- The only thing displayed to the user is the URL called. As I mentioned above, with a **GET** request the user will see the data in their URL bar, but with a **POST** request they won't. This can be very important for two reasons:  
    - If you need to send a password (or any other sensitive piece of data), never use the GET method or you risk displaying it in the URL bar, which would be very insecure.  
    - If you need to send a large amount of data, the POST method is preferred because some browsers limit the sizes of URLs. In addition, many servers limit the length of URLs they accept.  

**Retrieving Data**  
- Whichever HTTP method you choose, the server receives a string that will be parsed in order to get the data as a list of key/value pairs. The way you access this list depends on the development platform you use and on any specific frameworks you may be using with it.  
- PHP offers some global objects to access the data. Assuming you've used the POST method, the following example just takes the data and displays it to the user. Of course, what you do with the data is up to you. You might display it, store it into a database, send it by email, or process it in some other way.  

**Sending Files**  
- Sending files with HTML forms is a special case. Files are binary data — or considered as such — whereas all other data is text data. Because HTTP is a text protocol, there are special requirements for handling binary data.  

**Security**  
- Each time you send data to a server, you need to consider security. HTML forms are by far the most common server attack vectors (places where attacks can occur). The problems never come from the HTML forms themselves — they come from how the server handles data.  
