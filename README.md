# Emerging Media Lab Agora.io template

##How to get Agora.io working with Unity:

1. Create a new Unity project.
2. Using Unity's Package Manager, download and install the Agora.io video package.
3. Open File > Build Settings and add both "SceneHome" and "SceneHelloVideo" to "Scenes in Build".
4. Log into Agora.io. (If you don't have the EML Agora.io credentials, ask an EML staff member.)
5. In the Console/Dashboard, make sure you're on the "Overview" tab. Then under "Project Management", click "More". 
6. Select an existing project or create a new project, then click "Config" for that proiject under "Config" in the right hand column. (Ideally, you should use an existing one, because our free license only allows for a maximum of 20 projects INCLUDING DELETED PROJECTS.)
7.  Under "Security", turn on "Secondary Certificate". This enables "Temp token for audio/video call". IMPORTANT: Certificates and Tokens are different things!
8. Click "Generate temp RTC Token". Copy the resulting token to your clipboard.
9. In Unity, edit TestHelloUnityVideo.cs. On Line 22, change 'private string token = "";'
to:
'private string token = "REPLACE_THIS_WITH_YOUR_TOKEN";'
10. Open the scene TestHome and click "play". The game will change scenes to TestHelloUnityVideo. (Do not start from TestHelloUnityVideo.)
11. Success! Your computer's camera should automatically be detected, and your video should appear on the objects in the scene.
