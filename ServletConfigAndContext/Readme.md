# ServletConfig And Context

* **ServletConfig:**
  - ServletConfig is used to provide configuration information to a particular servlet. It contains initialization parameters specific to that servlet and allows the servlet to communicate with the servlet container about its configuration.
  - Key Characteristics:
      - Servlet-specific: Each servlet has its own ServletConfig object.
      - Initialization Parameters: ServletConfig allows a servlet to access its initialization parameters that are specified in the web.xml file.
      - Access to ServletContext: Through ServletConfig, you can access the ServletContext.


* **ServletContext:**
   - It is an application-wide object that is shared by all servlets within the web application. It allows servlets to interact with the servlet container and provides information about the web application as a whole.
   - Key Characteristics:
       - Application-wide: All servlets in a web application share the same ServletContext object.
       - Global Initialization Parameters: ServletContext can store global parameters accessible to all servlets.
       - Resource Access: ServletContext can be used to access resources like files, images, or even server-side configuration files.


* Difference Between `ServletConfig` and `ServletContext`

| Feature                | `ServletConfig`                        | `ServletContext`                      |
|------------------------|----------------------------------------|---------------------------------------|
| **Definition**         | Contains configuration information specific to a single servlet. | Provides information about the web application as a whole. |
| **Scope**              | Limited to the servlet for which it is created. | Shared across all servlets and JSPs in the web application. |
| **Initialization Parameters** | Allows defining initialization parameters for a servlet in `web.xml` or via annotations. | Allows defining context-wide parameters accessible by all servlets within the same web application. |
| **Access Method**      | Obtained using `getServletConfig()` method within the servlet. | Obtained using `getServletContext()` method from any servlet. |
| **Use Cases**          | Useful for servlet-specific settings, such as database connection parameters or file paths. | Useful for application-wide settings, such as configuration values, logging, or resources shared across servlets. |
