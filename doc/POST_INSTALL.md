1. Allow your domain
Edit the file /var/www/appflowy/appflowy_web/vite.config.ts by adding this option:
`  preview: {
    allowedHosts: ['__DOMAIN__'],
  },
`

2. Access
The admin panel (Appflowy-Cloud) can be accessed at https://__DOMAIN__/console/web/login

The web application (Appflowy-Web) can be accessed at https://__DOMAIN____PATH__

3. (Optional) Using a desktop client with your self-hosted Appflowy
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