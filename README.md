
![Logo](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

    
# thinkAR

An Augmented Reality & Artificial Intelligence mobile app for Design Thinking and brainstorming.

Recent transitions to working from home exposed the challenges surrounding remote collab- orative brainstorming. Existing ideation tools have concentrated predominantly on variants of digital whiteboard designs. Despite research suggesting that brainstorming in open settings with three-dimensional objects may yield more creative results, the role of Augmented Reality (AR) in ideation tools has remained largely unexplored.
This project aims to investigate the extent to which AR can facilitate the design thinking process. A prototype realised a three-dimensional interpretation of core design thinking concepts based on AR design principles. thinkAR is an Android and iOS mobile application based on Unity’s hybrid AR Foundation framework with a Node-RED and IBM Cloudant back end including IBM Watson services. The result demonstrates the feasibility of designing usable AR brainstorming and design thinking applications. The prototype may lay the groundwork for subsequent user acceptance research examining the relationship between AR and creativity.

## Demo

Insert gif or link to demo

  
## Authors

- [@benediktkau](https://www.github.com/benediktkau)

  
## Running Tests

To run tests, run the following command

```bash
  npm run test
```

  
## Screenshots

![App Screenshot](https://github.com/benediktkau/thinkAR/blob/main/res/screenshots/screenshot_avatars.jpg)

  
## Deployment

### Front end

<details>
<summary>Title 1</summary>
<p>
1. Create an empty Unity 3D project
2. Install all packages from the manifest.json
3. Follow all steps to set up the AR Foundation environment: https://learn.unity.com/ tutorial/setting-up-ar-foundation#5fe2be51edbc2a1f5e698730
4. Import Prefabs, Scenes, Scripts and UI into your empty project
5. Import the Microsoft Rocketbox avatars into a Unity Resources folder: https://github.
com/microsoft/\textit{Microsoft}-Rocketbox
6. [optional] Import animations into a Unity Resources folder: Mixamo.com
7. Import the Watson Developer Cloud Unity SDK: https://github.com/watson-developer-cloud/ unity-sdk
8. Import the Unity SDK Core: https://github.com/\textit{IBM}/unity-sdk-core
9. Import emojis for the avatars: https://openmoji.org/
10. Import icons for the UI: https://github.com/tabler/tabler-icons
After the backend has been set up:
1. Find the Login GameObject and enter the URL to your API into the field ”api” of the
MainMenu.cs file (see Figure A.1)
2. Find the SpeechToText GameObject and enter all IAM authentication credentials for the
Watson service into the fields (see Figure A.2)
3. Find the ToneAnalyzer GameObject and enter all IAM authentication credentials for the
Watson service into the fields (see Figure A.3).
</p>
</details>


## 🚀 About Me
I'm a full stack developer...

  
