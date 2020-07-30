# Deployment

### Install Firebase CLI using npm

First, install the firebase CLI

```text
npm install -g firebase-tools
```

### Before Deployment

{% hint style="danger" %}
Before build, make sure your backend api is correctly set up.
{% endhint %}

To set up backend api, go to **.env** file under the project directory, as change the **REACT\_APP\_BACKEND\_API\_KEY** to your deployed backend api.

Build your react app 

```text
npm run build
```

### Login to Firebase

Next associate the Firebase CLI with a Firebase account \(Google account\):

```text
firebase login
```

### Init project

Next, move to the project's folder and execute the following command, which initializes a Firebase project for the Firebase hosting features:

```text
firebase init
```

Then, choose the Hosting option. If you are interested in using another tool to host your Firebase application, choose another option:

![](../.gitbook/assets/k-opyqt-fxr-q330-jwnjtt.png)

Select your Firebase project from a list of projects from the Firebase platform

![](../.gitbook/assets/image%20%281%29.png)

 Use the _build/_ folder

![](../.gitbook/assets/image%20%283%29.png)

### Deploy

```text
Firebase deploy
```

