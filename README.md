# RESTful Web Services

### Date:17-05-2025

## Aim

To create RESTful web services using both server-side and client-side implementations.

## Procedure

### Server-Side Implementation

1. **Create a New Java Web Project:**
   - Follow steps 1-5 from the SOAP-based Web Services section to set up a new Java Web Project.

2. **Create RESTful Web Services:**
   - Right-click on the project name and select `New` -> `RESTful Web Services from Patterns`.

   ![Screenshot 2025-05-17 000444](https://github.com/user-attachments/assets/19dbd993-b36a-4bed-934d-aa942c910542)


3. **Configure Resource:**
   - In the new window, select `Simple Root Resource` and click `Next`.
   - Provide a Resource Package name and choose `MIME Type` as `text/html`. Click `Finish`.

   ![Screenshot 2025-05-17 000555](https://github.com/user-attachments/assets/2ff1e50f-0d06-4d1e-8bdd-64fab4dd7d2c)

   

4. **Edit Resource:**
   - Two editing tabs will appear. Close `ApplicationConfig.java` and implement the required functionalities in `GenericResource.java`.
  
    ![Screenshot 2025-05-17 000708](https://github.com/user-attachments/assets/f7962f26-bd9b-4d6e-9f1a-bf5c2f45fe82)


5. **Modify Method:**
   - Alter the `getHtml()` method as needed.

6. **Build and Deploy:**
   - Save your project, clean and build it. Deploy your project to the server.

    ![Screenshot 2025-05-17 000757](https://github.com/user-attachments/assets/637cdeba-d02f-4dac-89bd-b980f345ece8)


7. **Test Your Web Service:**
   - Open a browser and type the URL `http://localhost:8080/project_name/webresources/generic?params=45&params=35` to test the web service functionality.

### Client-Side Implementation

1. **Create a New Java Web Project:**
   - Follow steps 1-5 from the SOAP-based Web Services section to set up a new Java Web Project.

2. **Create RESTful Java Client:**
   - Right-click on the project and select `New` -> `RESTful Java Client`.

     ![Screenshot 2025-05-17 000832](https://github.com/user-attachments/assets/3f220985-b2d2-4da6-b700-69c20b3d26f9)


3. **Configure Client:**
   - In the new window, provide a name for your client, a package name, and select `From Project` under the `Select the REST resource:` tab. Click `Browse` and select your RESTful resource. Click `OK`, then `Finish`.

4. **Edit Client Code:**
   - Modify the `getHtml()` method as required.
  
     ![Screenshot 2025-05-17 000942](https://github.com/user-attachments/assets/2c2473c4-efd9-4b14-83a6-9f74451e5512)


5. **Add JAR File:**
   - Right-click on the `Libraries` folder under your project and select `Add JAR/Folder`.
   - Navigate to where the `javax.ws.rs-api2.0.1.jar` file is located and add it.
  
    ![Screenshot 2025-05-17 001007](https://github.com/user-attachments/assets/e3a826bd-3003-4119-9f5e-a9528d2ae70d)



6. **Create JSP Page:**
   - Right-click on the `Web Pages` folder and select `JSP`.
   - Provide a name for the JSP page and click `Finish`.
  
     ![Screenshot 2025-05-17 001041](https://github.com/user-attachments/assets/b1ed83e0-87eb-4f3c-9507-220fc460fd90)


7. **Include Client Code in JSP:**
   - Edit the JSP page to include the necessary code for invoking the client Java code.
  
     ![Screenshot 2025-05-17 001110](https://github.com/user-attachments/assets/8a5e7a11-7630-495a-8bea-3acacdb5d605)


8. **Build and Run:**
   - Save the project, build it, and run the JSP file to see the output in a new browser window.
  
     ![Screenshot 2025-05-17 001135](https://github.com/user-attachments/assets/8d05a58f-e614-445b-889e-0ea1a387e5fb)

Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.

Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code. 

   ![Screenshot 2025-05-17 001309](https://github.com/user-attachments/assets/ce47f531-5752-48a4-98db-f9351dc70c12)

Step 11: Save the project and build it. Step 12: Run the JSP file and you should see the output in a new browser

    ![Screenshot 2025-05-17 001406](https://github.com/user-attachments/assets/4117e432-5075-46a1-b584-ba2f4b21f23a)




### Client-Side Remote Invocation (Optional)

1. **Adjust Client Configuration:**
   - Follow steps 1-5 from the Client-Side Implementation.
   - In the generated `NewJerseyClient.java` file, update `BASE_URI` from `private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources";` to `private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";`.

2. **Complete the Remaining Steps:**
   - Follow steps 6-12 from the Client-Side Implementation to finalize and test the remote client.

## Result

The implementation of RESTful web services using both server-side and client-side components was successfully created and executed.

