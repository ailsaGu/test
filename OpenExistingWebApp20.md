
## Walkthrough Steps

### Copy the projects to local machine 

1. Clone the Git repo in VS (https://github.com/v-yanlli/OpenExisting.git)

    ![Project template](_images/20_OpenExistingWebApp/proj_clone.PNG)

2.  Open Team Explorer, clone the repo under 'Local Git Repositories'. The cloned repo will show up in 'Solution Explorer - Folder View'

    ![Project template type](_images/20_SimpleWebAppWithEmptyTemplate/proj_template_type.PNG)

3. Navigate to the path and open the solution shown in the table above

4. Wait for package restore to complete, verify package restore completes successfully without any error

    - View Output window > package Manager pane in Output window will show restore status

    - Wait till package restore completes

    ![Verify message in Output](_images/20_SimpleWebAppWithEmptyTemplate/verify_output_info.PNG)

### Build the solution and run locally

1. Open Startup.cs, build the project. Verify no errors or warnings in the output window and in the error list

    ![Build and verify error list](_images/20_SimpleWebAppWithEmptyTemplate/build_verify_errorlist.PNG)

2. F5 / Ctrl-F5 to run the project locally and verify page loads in the browser

### Publish to Azure

1. Right-click project > Publish

2. Provision a new Web App (Azure App Service) along with a SQL Azure DB in Azure and publish to it

    ![Add code in Configure method](_images/20_SimpleWebAppWithEmptyTemplate/add_usefileserver_in_configure.PNG)    


3. Verify publish succeeds and the page loads in the browser for the published site 

    ```
    <div>
        <p>Hello from HTML page</p>
    </div>
    ```

    ![Add content to index.html file](_images/20_SimpleWebAppWithEmptyTemplate/add_content_to_index.PNG)
    
3. Register a new user on the published site and log in


### Publish to Azure - Create a new web app on Azure and publish this project to Azure

1. Right-click project > Publish, choose Azure App Service > Create New

2. Create New Web app in existing or new Resource Group / App Service Plan, no database needed for this project

    ![Publish the project](_images/20_SimpleWebAppWithEmptyTemplate/proj_publish_new.PNG)

3. Click Settings link in Publish pane, navigate to Connection tab > Validate Connection

    ![Verify the validate connection](_images/20_SimpleWebAppWithEmptyTemplate/publish_validate_connection.PNG)

4. Navigate to Settings tab, pick the default options, select "Remove additional files at destination" and click Save

    ![Check the checkbox in Setting tab](_images/20_SimpleWebAppWithEmptyTemplate/publish_settings.PNG)

5. Click Preview link in Publish pane, click Start Preview

    ![Preview](_images/20_SimpleWebAppWithEmptyTemplate/publish_preview.PNG)

6. Publish to Azure, verify index.html page loads properly on published Azure site. 

    ![Verify index.html page loads properly after publish](_images/20_SimpleWebAppWithEmptyTemplate/publish_default.PNG)

   
### Publish to Azure again

1. Click Preview link in Publish pane > Preview changes

2. Publish to Azure again, verify bootstrap-styled page shows up in the published Azure site, and you can still 

    ![Verify bootstrap-styled shows up in Azure site](_images/20_SimpleWebAppWithEmptyTemplate/publish_target_default.png)

    
