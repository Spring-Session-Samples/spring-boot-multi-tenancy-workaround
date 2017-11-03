How to Executer this application

1.  clean this project first, Right click project >> Run As >> Maven Clean.
2.	update this maven project by right click on project >> Maven >> Update Project.
3.  Now, open `Application.java` & run as Java Application.
4.  You can change port number by opening `application.properties` file.
	top of this properites contains server.port, like wise can change data source info also.
	
4.	** Start POSTMAN & add header for any request about list, save, delete.
		** Header Name -  `X-TenantID`
		** Header Value - `tenant1`   [ any tenant value to use as tenant identification]  
5.  Send get request to get list of users of particular tenant as
        ** `http://localhost:8090/api/users`   
6.  To add a user, send post request with user bo body in json as
		{
		    "username": "demo",
		    "firstName": "krishna",
		    "lastName": "mohan"
		}

7.  Please check other option as well in UserController.java

Thanks for using this application.