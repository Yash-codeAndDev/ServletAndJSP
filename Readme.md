# Servlet and JSP

* **Servlet** :  Servlets are Java programs that run on a web server and act as intermediaries between client requests and server responses. They are used to create dynamic web content and handle HTTP requests (such as GET, POST, PUT, DELETE) and generate responses in various formats like HTML, XML, JSON, etc.
  * Key Features of Servlet :
      - Platform Independence: Servlets are platform-independent and can run on any server that supports the Servlet API.

      - Request-Response Model: Servlets follow the client-server architecture, where they handle HTTP requests (like form submissions, URL requests) and respond back with dynamic content (like web pages, data, etc.).

      - Efficiency: Servlets are efficient in handling multiple requests concurrently. One instance of a servlet can handle multiple requests, reducing the memory and resource footprint.

      - Lifecycle Management: The servlet container (like Tomcat) manages the lifecycle of a servlet, handling its creation, request processing, and destruction automatically.

      - Session Management: Servlets can maintain session data between requests using techniques like HTTP sessions, cookies, or URL rewriting.

* **Servlet Lifecycle**
