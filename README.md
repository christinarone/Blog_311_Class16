# Blog_311_Class16
Class 16
Can you explain the purpose of each type of HTTP Request when using a RESTful web service?
  1. GET

Retrieves data from the server (should only retrieve data and should have no other effect). This is also called an idempotent method. here is an example of a GET request to retrieve the book with id 123 from Server.

GET /books/123

2. POST

This HTTP request type is usually used for creating an entity i.e. a resource without an id. Once the request is successfully created, an id of the newly created entity is returned as part of the response to this HTTP request. It is often used when uploading a file or submitting a completed web form.

For example, following URL will create a new book in the server

POST /books/

3. PUT

Similar to POST, but used to update an existing entity. You pass the id of existing resource along with PUT request type. For example, following URL will replace the book with id 123 in the server

PUT /books/123

4. DELETE

Removes the resource from the server. Similar to PUT you need to pass the id of the resource to be deleted. For example, following URL will remove the book with id 123 in the server

DELETE /books/123

What's a test pyramid? How can you implement it when talking about HTTP APIs?
  It is a concept that is used to describe the number of different types of tests visually. Test types are sorted so that the base is represented by the test type of the highest quantity. Moving higher in the pyramid, each level is represented by the type with the lower number of tests.
  
What is the "demultiplexer"?
  The demultiplexer is a combinational logic circuit designed to switch one common input line to one of several seperate output line.
  
What’s the difference between "blocking" and ‘non-blocking’ functions?
  Blocking refers to operations that block further execution until that operation finishes while non-blocking refers to code that doesn't block execution. 
  
What are the main security implementations within NodeJS?
  These include SQL Injection, Cross-Site Scripting, Command Injection, Local/Remote File Inclusion, Denial of Service, Directory Traversal, LDAP Injection and many other injection attacks. In order to avoid these attacks, input to your application should be sanitized first.
  
Explain the “path” module in NodeJS.
  Node. js provides you with the path module that allows you to interact with file paths easily. The path module has many useful properties and methods to access and manipulate paths in the file system. The path is a core module in Node.
