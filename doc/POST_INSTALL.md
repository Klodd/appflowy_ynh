1. **Allow your domain**
Edit the file /var/www/appflowy/appflowy_web/vite.config.ts by adding this option:
`  preview: {
    allowedHosts: ['__DOMAIN__'],
  },
`
2. **Restart the Web service**
`service appflowy_web restart`

3. **Access to admin panel**
The admin panel (Appflowy-Cloud) can be accessed at https://__DOMAIN__/console/web/login

You will not be able to use the (Appflowy-web) Webapp client yet (see step 5)

4. **Use a desktop client with your self-hosted Appflowy**
Download and install the AppFlowy application for you device: https://appflowy.io/downloaded
Open the AppFlowy application.
Click on 'Quick Start'.
Navigate to the `Settings` page.
On the left sidebar, select `Cloud Setting`.
Choose `AppFlowy Cloud` as your cloud provider.
Enter your server address <https://__DOMAIN____PATH__> in the provided field.
Click Restart to apply the changes.
Go the `Setting` page
On the left sidebar, select `User`

5. **Connect to the appflowy web app**
The web application (Appflowy-Web) can be accessed at https://__DOMAIN____PATH__

> A new user must connect through the native app for first login (this is a bug I encountered, personal workspace creation does not happen in the browser app, only when connecting with a native app)
