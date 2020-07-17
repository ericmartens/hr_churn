## Accounts and services

1. Sign up for a free [IBM Cloud account](https://cloud.ibm.com/).
2. Sign up for a free [Watson Studio account](https://dataplatform.ibm.com/).
3. Provision a free lite instance of [Watson Machine Learning](https://cloud.ibm.com/catalog/services/machine-learning). **Choose either the Dallas or Frankfurt region.**
4. Provision a free lite instance of [Watson OpenScale](https://cloud.ibm.com/catalog/services/watson-openscale). **Choose the same region (Dallas or Frankfurt) you selected for Watson Machine Learning.** You just need to provision the service for now. **DO NOT RUN THE AUTO-SETUP DURING THE WEBCAST.** It will take too much time to complete and you won't be able to follow along.
5. Provision a free instance of [Object Storage](https://cloud.ibm.com/catalog/services/cloud-object-storage).

## Setup
In this step, you will create the service credentials and projjects you need for the hands-on lab.

Start by creating credentials for Watson Machine Learning. Navigate to your [IBM Cloud Resources page](https://cloud.ibm.com/resources). From the **Resource list**, expand the **Services** section and click on the instance of Watson Machine Learning you created in the previous section.

![Resource list -> Services -> Watson Machine Learning](./img/step_00/find_wml.png)

From the menu on the left, click on **Service credentials**.

![Service credentials](./img/step_00/service_credentials.png)

Click blue the **New credential** button.

![New credential](./img/step_00/new_credential.png)

Give your credentials a name, and then click the **Add** button.

![Add credential](./img/step_00/add_credential.png)

Your new credentials will appear in the list. Click the **copy button** to copy them to your clipboard.

![Copy to clipboard](./img/step_00/copy_credentials.png)

Open your favorite text editor and paste the credentials into a new file. We will use them in a few different locations in later steps.

Next, you'll need a Cloud API key. Navigate to the [Cloud user API key page](https://cloud.ibm.com/iam/apikeys) and click the **Create an IBM Cloud API key** button.

![Create an IBM Cloud API key](./img/step_00/create_api_key.png)

Give your key a name and click the **Create** button.

![Confirm API key creation](./img/step_00/create_api_confirm.png)

Click the **Copy** button to copy the key to your clipboard.

![Copy API key](./img/step_00/copy_api_key.png)

Paste the API key into your text editor file for later use.

Finally, you will need to create a Watson Studio project for your Python notebooks and models. Navigate to the [Watson Studio home page](https://dataplatform.cloud.ibm.com/) and click the **New project** button.

![New project](./img/step_00/new_project.png)

Click the **Create an empty project** tile.

![Empty project](./img/step_00/empty_project.png)

Give your project a name. In the **Define storage** section, select the Object Storage instance you created in the previous section, and then click **Create**.

![Project details](./img/step_00/project_details.png)

Click on the **Settings** tab at the top of the screen.

![Project settings](./img/step_00/settings.png)

Scroll down to the **Associated services** section. Click the **Add service** button and select **Watson** from the list.

![Associate Watson services](./img/step_00/add_service.png)

Click the **Add** button on the **Machine Learning** tile.

![Add Machine Learning](./img/step_00/machine_learning.png)

Select the instance of Watson Machine Learning you created in a previous step from the dropdown, and click the **Select** button.

![Existing service instance](./img/step_00/existing_service_instance.png)

You are now ready to create a Watson Sudio project and run the notebooks.
