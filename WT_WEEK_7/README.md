### Greeting's Web Application

- Firstly, create a `HTML` file named as `welcome_servlet.html` (The name of `HTML` file can be anything but, better to keep an easy one).
- Secondly, create a `Java` file named as `WelcomeServlet.java` (This name should be absolute no changes, if you done any make sure to change in the `HTML` file too)
- Now, Start the Tomcat server but double clicking `Tomcat10.exe` and leave the cmd window be.
- **Path to find Tomcat10.exe is** [`Program Files\Apache Software Foundation\Tomcat 10.1\bin`]()
- After that, double click the `startup.bat` for our benefit.
- Place the `welcome_servlet.html` in this path [`Program Files\Apache Software Foundation\Tomcat 10.1\webapps\examples`]()
- Now, compile the `WelcomeServlet.java` and then a class file is generated `WelcomeServlet.class` place these two file in (classes folder) this path [`Program Files\Apache Software Foundation\Tomcat 10.1\webapps\examples\WEB-INF\classes`]()
- Update the existing `web.xml` available in the path `` with the below data

```xml
<servlet>
        <servlet-name>WelcomeServlet</servlet-name>
        <servlet-class>WelcomeServlet</servlet-class>
</servlet>
<servlet-mapping>
        <servlet-name>WelcomeServlet</servlet-name>
        <url-pattern>/WelcomeServlet</url-pattern>
</servlet-mapping>
```

- Let's execute the program by going to the tomcat server by typing [`http://localhost:8080`]() in the browser address bar.
- Now in the address bar replace it with this url [`http://localhost:8080/examples/welcome_servlet.html`]()
- That's it now you can access the web application with ease.

<font color="red">Note : </font>

- Donot close the cmd window that appeared when you clicked the `Tomcat10.exe`