
```
npm install -g @aws-amplify/cli
amplify configure
```


### How to get aws key
1. Log in to your AWS Management Console.
2. Click on your user name at the top right of the page.
3. Click on the Security Credentials link from the drop-down menu.
4. Find the Access Credentials section, and copy the latest Access Key ID.
5. Click on the Show link in the same row, and copy the Secret Access Key.


```
amplify init
```


### Tips

Some next steps:
1. "amplify status" will show you what you've added already and if it's locally configured or deployed
2. "amplify <category> add" will allow you to add features like user login or a backend API
3. "amplify push" will build all your local backend resources and provision it in the cloud
4. "amplify publish" will build all your local backend and frontend resources (if you have hosting category added) and provision it in the cloud

Pro tip:
1. Try "amplify add api" to create a backend API and then "amplify publish" to deploy everything


After you answer the provided questions, you can use ```amplify help```  at any time to see the overall command structure, and ```amplify help   <category>``` to see actions for a specific category.


### Publishing Your Web App
```
amplify add hosting
```

You would be prompted next to select the environment setup. Select DEV (S3 only with HTTP) for quick prototyping and testing, and once production ready you could run the amplify update hosting command to publish your app to Amazon CloudFront (a CDN service).