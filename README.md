
![Logo](https://github.com/benediktkau/thinkAR/blob/main/res/logo.png)

    
# thinkAR - AR Brainstorming Mobile App

An Augmented Reality & Artificial Intelligence Mobile Application for Design Thinking

**thinkAR** is an Android and iOS mobile application based on Unity’s hybrid AR Foundation framework with a Node-RED and IBM Cloudant back end including IBM Watson services. The result demonstrates the feasibility of designing usable AR brainstorming and design thinking applications. The prototype may lay the groundwork for subsequent user acceptance research examining the relationship between AR and creativity.

  
<details>
<summary>Context & Background</summary>
<p>thinkAR is an Android and iOS mobile application based on Unity’s hybrid AR Foundation framework with a Node-RED and IBM Cloudant back end including IBM Watson services. The result demonstrates the feasibility of designing usable AR brainstorming and design thinking applications. The prototype may lay the groundwork for subsequent user acceptance research examining the relationship between AR and creativity.</p>
 </details>

  
## Authors

- [@benediktkau](https://www.github.com/benediktkau)
  
## Screenshots

![App Screenshot](https://github.com/benediktkau/thinkAR/blob/main/res/screenshots/screenshot_avatars.jpg)

![App Screenshot](https://github.com/benediktkau/thinkAR/blob/main/res/screenshots/screenshot_avatars.jpg)

![App Screenshot](https://github.com/benediktkau/thinkAR/blob/main/res/screenshots/screenshot_avatars.jpg)

  
## Deployment

### 📱 Front end

1. Create an empty Unity 3D project
2. Install all packages from the manifest.json
3. Follow all steps to set up the [AR Foundation](https://learn.unity.com/tutorial/setting-up-ar-foundation#5fe2be51edbc2a1f5e698730 "Unity AR Foundation") environment
4. Import Prefabs, Scenes, Scripts and UI into your empty project
5. Import the  [Microsoft Rocketbox](https://github.com/microsoft/\textit{Microsoft}-Rocketbox "Microsoft Rocketbox") avatars into a Unity Resources folder.
6. Import [animations](https://Mixamo.com "Mixamo Animations") into a Unity Resources folder.
7. Import the [Watson Developer Cloud Unity SDK](https://github.com/watson-developer-cloud/unity-sdk "Watson Developer Cloud Unity SDK").
8. Import the [Unity SDK Core](https://github.com/\textit{IBM}/unity-sdk-core "Unity SDK Core").
9. Import [emojis](https://openmoji.org/ "OpenMoji") for the avatars.
10. Import [icons](https://github.com/tabler/tabler-icons "TablerIcons") to beautify the user interface.
After the backend has been set up:
1. Find the ```Login``` GameObject and enter the API URL into the Serialized Field ```api``` of
```MainMenu.cs```.
2. Find the ```SpeechToText``` GameObject and enter the IAM authentication credentials for the
Watson service into the Serialized Fields.
3. Find the ```ToneAnalyzer``` GameObject and enter the IAM authentication credentials for the
Watson service into the Serialized Fields.

### 🔨 Back end

1. Create an [IBM Cloud](https://cloud.ibm.com/ "IBM Cloud") account.
2. Set up a Node-RED instance as a Cloud Foundry app on IBM Cloud. [This tutorial](https://cognitiveclass.ai/badges/node-red-basics-to-bots "Node-RED Basics to Bots Tutorial") might be helpful. 
3. The Node-RED instance will automatically set up and connect to an IBM Cloudant instance.
4. Import ```flows.json``` into Node-RED.
5. In the Cloudant dashboard, create databases with the names: ```users```, ```projects```, ```empathise```, ```ideate```. You may use names different from these, but do not forget to change the names in the Node-RED Cloudant nodes 😉.
6. For each Cloudant database, create a search index and copy & paste each the corresponding design documents (not the documents themselves) from Section C.2
7. Create an IBM Watson Speech to Text application on IBM Cloud and share the credentials with Unity (see front end description)
8. Create an IBM Watson Tone Analyzer application on IBM Cloud and share the credentials with Unity (see front end description)


## 🚀 About Me
UCL MSc Computer Science • Thesis @IBM • 💙 Product Fellow @Tech4Germany • Previously Digitalisation @Deutsche Bahn & Business Development @VW New Mobility Services Beijing
