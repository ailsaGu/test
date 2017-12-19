
## Walkthrough Steps

### Clone the Git repo in VS 

1. Open Team Explorer, clone the repo under 'Local Git Repositories'.(https://github.com/v-yanlli/OpenExisting.git)

    ![Project template](_images/20_OpenExistingWebApp/proj_clone.PNG)

2.   The cloned repo will show up in 'Solution Explorer - Folder View'.

     ![Project template](_images/20_OpenExistingWebApp/proj_repo.PNG)

3. Navigate to the path and open the project in OpenExistingAspNetCore2xFromSC folder as shown in the table above

4. Wait for package restore to complete, verify package restore completes successfully without any error

    - View Output window > package Manager pane in Output window will show restore status

    - Wait till package restore completes

    ![Verify message in Output](_images/20_OpenExistingWebApp/verify_output_info.PNG)

### Build the solution and run locally

1. Open Startup.cs, build the project. Verify no errors or warnings in the output window and in the error list

    ![Build and verify error list](_images/20_OpenExistingWebApp/build_verify_errorlist.PNG)

2. F5 / Ctrl-F5 to run the project locally and verify page loads in the browser

### Publish to Azure - Create a new web app on Azure and publish this project to Azure

1. Right-click project > Publish, choose Azure App Service > Create New

2. Create New Web app in existing or new Resource Group / App Service Plan. (If you publish a project with InAuth, Provision a database as well in the "Services" tab)

    ![Publish the project](_images/20_OpenExistingWebApp/proj_publish_new.PNG)

3. Click Settings link in Publish pane, navigate to Connection tab > Validate Connection

    ![Verify the validate connection](_images/20_OpenExistingWebApp/publish_validate_connection.PNG)

4. Navigate to Settings tab, pick the default options, select "Remove additional files at destination" and click Save. (If you publish a project with InAuth, select EF )

    ![Check the checkbox in Setting tab](_images/20_OpenExistingWebApp/publish_settings.PNG)

5. Click Preview link in Publish pane, click Start Preview

    ![Preview](_images/20_OpenExistingWebApp/publish_preview.PNG)

6. Publish to Azure, verify index.html page loads properly on published Azure site. 

    ![Verify index.html page loads properly after publish](_images/20_OpenExistingWebApp/publish_default.png)

7. If you publish a project with InAuth,  Register a new user on the published site and log in .


    
