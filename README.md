# RESTful Web Services

### Date: 15/05/2025

## Aim

To create RESTful web services using both server-side and client-side implementations.

## Procedure

### Server-Side Implementation

1. **Create a New Java Web Project:**
   - Follow steps 1-5 from the SOAP-based Web Services section to set up a new Java Web Project.

2. **Create RESTful Web Services:**
   - Right-click on the project name and select `New` -> `RESTful Web Services from Patterns`.
![EXPERIMENT 4](https://github.com/user-attachments/assets/b74e9f9f-2ffc-4859-96c5-9c67af3c3835)
     
3. **Configure Resource:**
   - In the new window, select `Simple Root Resource` and click `Next`.
   - Provide a Resource Package name and choose `MIME Type` as `text/html`. Click `Finish`.
![EXPERIMENT 4 (1)](https://github.com/user-attachments/assets/04ae2730-1348-44ba-ac5a-6f57a8c64999)

4. **Edit Resource:**
   - Two editing tabs will appear. Close `ApplicationConfig.java` and implement the required functionalities in `GenericResource.java`.
![EXPERIMENT 4 (2)](https://github.com/user-attachments/assets/d018b8ef-3f20-4e71-9f41-e1d3fea5e9c4)

5. **Modify Method:**
   - Alter the `getHtml()` method as needed.

6. **Build and Deploy:**
   - Save your project, clean and build it. Deploy your project to the server.
![EXPERIMENT 4 (3)](https://github.com/user-attachments/assets/a5cf267b-7218-4964-bcca-7be6a0ad2b2e)

7. **Test Your Web Service:**
   - Open a browser and type the URL `http://localhost:8080/project_name/webresources/generic?params=45&params=35` to test the web service functionality.

### Client-Side Implementation

1. **Create a New Java Web Project:**
   - Follow steps 1-5 from the SOAP-based Web Services section to set up a new Java Web Project.

2. **Create RESTful Java Client:**
   - Right-click on the project and select `New` -> `RESTful Java Client`.
![EXPERIMENT 4 (4)](https://github.com/user-attachments/assets/b3dcf83d-0f4a-45c6-9568-c207f43db040)

3. **Configure Client:**
   - In the new window, provide a name for your client, a package name, and select `From Project` under the `Select the REST resource:` tab. Click `Browse` and select your RESTful resource. Click `OK`, then `Finish`.

4. **Edit Client Code:**
   - Modify the `getHtml()` method as required.
![EXPERIMENT 4 (5)](https://github.com/user-attachments/assets/5b288272-b68b-408b-bf79-1b1579462f92)

5. **Add JAR File:**
   - Right-click on the `Libraries` folder under your project and select `Add JAR/Folder`.
   - Navigate to where the `javax.ws.rs-api2.0.1.jar` file is located and add it.
![EXPERIMENT 4 (6)](https://github.com/user-attachments/assets/36ee5626-286d-4d02-9955-84efad5347ee)

6. **Create JSP Page:**
   - Right-click on the `Web Pages` folder and select `JSP`.
   - Provide a name for the JSP page and click `Finish`.
![EXPERIMENT 4 (7)](https://github.com/user-attachments/assets/7b7c2b33-5ebd-457f-b4f8-e63dc8391b71)

7. **Include Client Code in JSP:**
   - Edit the JSP page to include the necessary code for invoking the client Java code.
![EXPERIMENT 4 (8)](https://github.com/user-attachments/assets/a2377dfb-7580-42b9-8cd7-0e2f7a555dc2)

8. **Build and Run:**
   - Save the project, build it, and run the JSP file to see the output in a new browser window.
![EXPERIMENT 4 (9)](https://github.com/user-attachments/assets/9cf7b356-b81d-49fd-a6f6-315981dae772)

Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.

Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.
![EXPERIMENT 4 (10)](https://github.com/user-attachments/assets/3fed2bcc-ca99-454c-896f-33691dacd378)

Step 11: Save the project and build it. Step 12: Run the JSP file and you should see the output in a new browser window.
![EXPERIMENT 4 (11)](https://github.com/user-attachments/assets/68cfa17e-f5b6-4d07-96e3-830d0da94e62)


### Client-Side Remote Invocation (Optional)

1. **Adjust Client Configuration:**
   - Follow steps 1-5 from the Client-Side Implementation.
   - In the generated `NewJerseyClient.java` file, update `BASE_URI` from `private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources";` to `private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";`.

2. **Complete the Remaining Steps:**
   - Follow steps 6-12 from the Client-Side Implementation to finalize and test the remote client.

## Result

The implementation of RESTful web services using both server-side and client-side components was successfully created and executed.

