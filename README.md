# RESTful Web Services

### Date:

## Aim

To create RESTful web services using both server-side and client-side implementations..

## Procedure

### Server-Side Implementation

1. **Create a New Java Web Project:**
   - Follow steps 1-5 from the SOAP-based Web Services section to set up a new Java Web Project.

2. **Create RESTful Web Services:**
   - Right-click on the project name and select `New` -> `RESTful Web Services from Patterns`.
   - ![image](https://github.com/user-attachments/assets/a15c8fa7-9dd3-455c-b83c-f010c32b7562)


3. **Configure Resource:**
   - In the new window, select `Simple Root Resource` and click `Next`.
   - Provide a Resource Package name and choose `MIME Type` as `text/html`. Click `Finish`.
   - ![image](https://github.com/user-attachments/assets/cfb5d512-b026-4ada-8aef-1552b220a32d)


4. **Edit Resource:**
   - Two editing tabs will appear. Close `ApplicationConfig.java` and implement the required functionalities in `GenericResource.java`.
   - ![image](https://github.com/user-attachments/assets/3b8afead-5bb9-4adb-a803-7fd61b817915)


5. **Modify Method:**
   - Alter the `getHtml()` method as needed.

6. **Build and Deploy:**
   - Save your project, clean and build it. Deploy your project to the server.
   - ![image](https://github.com/user-attachments/assets/f2bcacba-fe1c-4417-81d7-274c63a60005)


7. **Test Your Web Service:**
   - Open a browser and type the URL `http://localhost:8080/project_name/webresources/generic?params=45&params=35` to test the web service functionality.

### Client-Side Implementation

1. **Create a New Java Web Project:**
   - Follow steps 1-5 from the SOAP-based Web Services section to set up a new Java Web Project.

2. **Create RESTful Java Client:**
   - Right-click on the project and select `New` -> `RESTful Java Client`.
   - ![image](https://github.com/user-attachments/assets/89eeb661-ab7f-4ad4-ab68-b162532a20ed)


3. **Configure Client:**
   - In the new window, provide a name for your client, a package name, and select `From Project` under the `Select the REST resource:` tab. Click `Browse` and select your RESTful resource. Click `OK`, then `Finish`.

4. **Edit Client Code:**
   - Modify the `getHtml()` method as required.
   - ![image](https://github.com/user-attachments/assets/bbec8b64-c171-42b8-96a5-def309c73486)


5. **Add JAR File:**
   - Right-click on the `Libraries` folder under your project and select `Add JAR/Folder`.
   - Navigate to where the `javax.ws.rs-api2.0.1.jar` file is located and add it.
   - ![image](https://github.com/user-attachments/assets/92cfee98-f69d-4d75-be66-5d00edabeec8)


6. **Create JSP Page:**
   - Right-click on the `Web Pages` folder and select `JSP`.
   - Provide a name for the JSP page and click `Finish`.
   - ![image](https://github.com/user-attachments/assets/f61942a0-f901-4104-bec0-43837bc1793f)


7. **Include Client Code in JSP:**
   - Edit the JSP page to include the necessary code for invoking the client Java code.
   - ![image](https://github.com/user-attachments/assets/c0d584e9-69b2-4012-974b-05dcdbce37d4)


8. **Build and Run:**
   - Save the project, build it, and run the JSP file to see the output in a new browser window.
   - ![image](https://github.com/user-attachments/assets/9e88d433-8d59-41b5-b159-fdc2545ab21b)


### Client-Side Remote Invocation (Optional)

1. **Adjust Client Configuration:**
   - Follow steps 1-5 from the Client-Side Implementation.
   - In the generated `NewJerseyClient.java` file, update `BASE_URI` from `private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources";` to `private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";`.

2. **Complete the Remaining Steps:**
   - Follow steps 6-12 from the Client-Side Implementation to finalize and test the remote client.

## Result

The implementation of RESTful web services using both server-side and client-side components was successfully created and executed.

