## Part 1, create your application and development environment
1. Compress index.php that is in this repo and name that archive v1.zip
2. Click on services, and search for **Elastic Beanstalk** or select it from the list of services in the **Compute** section
3. Click **Create New Application** in the top left corner of your screen.
Name you application, and enter a useful description.
1. Click **Create One Now** to create a new environment in your application.
2. Leave **Web server environment** selected and click select.
3. Set up your environment.
    - Choose "PHP" for the preconfigured platform
    - At the bottom, choose upload your code and click 
    **Upload**
    - choose a local file and choose the v1.zip file ithat you created earlier
    - Change the version label to "V1" and click **Upload**
4. Click **Create Environment**

It will take approximately 5 minutes to create this simple environment. Once this is complete, your webpage will transition to the environment dashboard. You can click on the URL close to the top of the dashboard to see the simple web page that you are hosting.
___
## Part 2, Update your environment;Change your web application code and update your environment.

1. Open **index.php** in this folder.
2. Change line 12 from
```html
    <title>Hello World!</title>
```
To
```html
    <title>Hello AWS Students!</title>
```
And

```html
    <h1>Hello World!</h1>
```
To 
```html
    <h1>Hello AWS Students!</h1>
```
3. After saving the file, add **index.php** to a zip file in file browser of your choice. Rename that zip file to "V2.zip".
4. Back in the AWS Console, on your Environment Dashboard, Click **Upload and Deploy**
5. Click **Choose File**, choose "V2.zip" and click deploy.
6. This simple deploy will only take approximately 20 seconds.
7. Click on your URL at the top of the dashboar, or refresh the tab if you already have it in your browser, and you should see your new code.

### If for some reason you don't like this new verion of your application. Just roll it back!

1. Click on your application name in the top left corner of your browser, mine is **MCB Web Applicaiton**, and choose application versions.
2. Select "V1" (or any other version if there are more than one), and choose deploy.
> If you have more than one environment, you want to make sure that you choose the intended environment.
3. Just like before, the deployment shoud take about 20 seconds for this simple environment.
4. If you visit the URL for your environment you should see the original version of your code.