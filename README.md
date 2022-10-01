# admin-lte-servlet
This Project Describe how to Config AdminLte Template with Servlet and Jsp

How to config Admin Lte Templat with servlet and Jsp
Prerequisite
1. Understanding Admin Lte component
2. Understand the concept of breaking down Admin LTE into parts(header.jsp, menus.jsp, footer.jsp, and addition.jsp which contain javascript library)
3. Understanding concept templating(reuse header, menus, footer and addition.jsp in page which you create new page)
4. understanding to run app using embedded server(jetty, if not familiar see my previous tutorial)
5. download AdminLte template from github(https://github.com/ColorlibHQ/AdminLTE)


breaking down Admin Lte into parts
0. open index.html
1. header contain css which load into page
2. menus contain sidebar and header
3. content contain dynamic content(when creating new page replace according business rule)
4. footer contain footer description 
5. addition contain js library which load into page
6. When create new page include 5 fragment on above


Let's Jump right in
1. dependency and plugin which needed
2. this is my package structure
3. this is my resources folder(css, images, js)
4. create fragment folder to save(header, menus, footer, addition jsp)
5. create pages folder to save page with different content
6. open index.html Admin-Lte page
6. create header.jsp(i'm already created header.jsp) copy header from AdminLte to header.jsp
7. create menus.jsp(copy menus from adminLte to menus.jsp)
8. create footer.jsp(copy footer from adminLte to footer.jsp)
9. create addition.jsp(copy from AdminLte to addition.jsp)
10. copy all js, css, images needed to folder(css, js and images)
11. copy webfonts from adminLte template
12. add pageEncoding in above fragment
13. add jstl core in above fragment
14. create new page with name index_page, include all fragments and fill content form adminLte 
15. create new controller for handler request when user request home page(dashboard)
16. mapping request in web.xml
17. try to run app using this command  mvn jetty:run

Succed, Happy learning and happy sharing!!!
You can download this code, from my github

#How To Run
1. Import Project into intellij Idea
2. update pom.xml to download dependency from maven repository
3. run this command mvn jetty:run
4. hit this url http://localhost:8080/myWebApp/home-servlet
