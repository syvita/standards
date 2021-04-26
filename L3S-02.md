# C4model
C4model is a methodology to express software architectures in block diagram shapes...Kind of graphical notation or expressing language for modelling soft architectures.
## 1- First level of Visualization
The zoom-out perspective of the whole system in the biggest scale. Detail isn't important here as this is your zoomed out view showing a big picture of the system landscape. The focus should be on people (actors, roles, personas, etc) and software systems rather than technologies, protocols and other low-level details. It's the sort of diagram that you could show to non-technical people.

![c4model-1st%20level.png](c4model-1st%20level.png)

So in short, each shape demonstrates below meanings:
![c4model-1st%20level-2.png](c4model-1st%20level-2.png)
.
.
.                                                                                                                                                                                                                                                                                                                                                          

**example:**
This is an example System Context diagram for a fictional Internet Banking System. It shows the people who use it, and the other software systems that the Internet Banking System has a relationship with. Personal Customers of the bank use the Internet Banking System to view information about their bank accounts, and to make payments. The Internet Banking System itself uses the bank's existing Mainframe Banking System to do this, and uses the bank's existing E-mail System to send e-mails to customers.
![c4model-1st%20level-example.png](c4model-1st%20level-example.png)

## 2- Second level of visualization 
You zoom in a bit and you are in second level. This level of visualization is shown inside a dash-line boundry with **container** blocks.Once you understand how your system fits in to the overall IT environment, a really useful next step is to zoom-in to the system boundary with a Container diagram. 
                                                                                                                                                                                   ![c4model-2nd%20level.png](c4model-2nd%20level.png)                                                                                                                                                                       
**Example:**
This is an example Container diagram for a fictional Internet Banking System. It shows that the Internet Banking System (the dashed box) is made up of five containers: a server-side Web Application, a Single-Page Application, a Mobile App, a server-side API Application, and a Database. The Web Application is a Java/Spring MVC web application that simply serves static content (HTML, CSS and JavaScript), including the content that makes up the Single-Page Application. The Single-Page Application is an Angular application that runs in the customer's web browser, providing all of the Internet banking features. Alternatively, customers can use the cross-platform Xamarin Mobile App, to access a subset of the Internet banking functionality.

Both the Single-Page Application and Mobile App use a JSON/HTTPS API, which is provided by another Java/Spring MVC application running on the server. The API Application gets user information from the Database (a relational database schema). The API Application also communicates with the existing Mainframe Banking System, using a proprietary XML/HTTPS interface, to get information about bank accounts or make transactions. The API Application also uses the existing E-mail System if it needs to send e-mails to customers.

![c4model-2nd%20level-example.png](c4model-2nd%20level-example.png)

## 3- Third level of visualisation
You can zoom in more into level-2 containers/blocks. 
shows how a container is made up of a number of "components"....Symbol diagrams below listed: 
![c4model-3rd%20level.png](c4model-3rd%20level.png)

**Example:**
This is an example Component diagram for a fictional Internet Banking System, showing some (rather than all) of the components within the API Application. Here, there are three Spring MVC Rest Controllers providing access points for the JSON/HTTPS API, with each controller subsequently using other components to access data from the Database and Mainframe Banking System, or send e-mails.

![c4model-3rd%20level-example.png](c4model-3rd%20level-example.png)

## 4- Forth level of visualization
To zoom in to see the codes. This is an optional level of detail and is often available on-demand from tooling such as IDEs.

This is an example (and partial) UML class diagram for a fictional Internet Banking System, showing the code elements (interfaces and classes) that make up the MainframeBankingSystemFacade component. It shows that the component is made up of a number of classes, with the implementation details directly reflecting the code.
![c4model-4th%20level-example.png](c4model-4th%20level-example.png)
