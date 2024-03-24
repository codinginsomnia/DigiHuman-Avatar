Installation:

Backend Server Installation:

Install MediaPipe Python:
Copy code
pip install mediapipe
Install OpenCV Python:
Copy code
pip install opencv-python
Navigate to the backend directory and install other requirements:
Copy code
pip install -r requirements.txt
Download the pre-trained generator model for the COCO dataset and place it into backend/checkpoints/coco_pretrained/.
Unity3D Installation:

Download and install UnityHub.
Add a new license in UnityHub and register it.
Install a Unity Editor inside UnityHub (LTS versions and a version higher than 2020.3.25f1 are recommended).
In the Unity project settings, allow HTTP connections in the player settings.
Usage:

Run the backend server at the backend directory with the following command:
Copy code
python server.py
Run the Unity project and open the main scene at Assets\Scenes\MainScene.unity.
Test the program by uploading videos to the backend from the Unity project (You can test the application by selecting provided animations from the right-side menu).
Adding New 3D Characters:

Find a 3D character model from the Unity asset store or download a free one.
Set the rig to humanoid in the character settings.
Drag and drop your 3D character model to CharacterChooser/CharacterSlideshow/Parent object in Unity main Scene.
Add BlendShapeController and QualityData components to the character object in the scene.
Set BlendShapeController values and add character SkinnedMeshRenderer component to BlendShapeController component.
Add the character to the nodes property of CharacterSlideshow Object.
Run the application and select your character for rendering animation.
Features:

Making full body animation.
Animating multiple blendShapes on 3D character (up to 40 blendshape animations are supported currently).
Supporting any 3D models with Humanoid T-Pose rig.
Exporting animation in a video file.
Saving animation data and re-rendering it for future usage.
Filtering MediaPipe outputs to detect and remove noises and better smoothness (Low Pass Filtering is used currently).
Animating the character's face in great detail.
Training a regression model to generate Blendmesh weights by feeding the output data of MediaPipe FaceMesh (468 points).
Using StyleGan techniques to replace the whole character face mesh.
Automatic rigging for 3D models without a humanoid rig (Using deep neural network models like RigNet).
Generating a complete character mesh automatically using models like PIFuHD (in progress!).
Animating the 3D character's mouth in great detail using audio signal or natural language processing methods.
Generating a complete environment in 3D.
User
don't have code snippets i want the same in text
ChatGPT
Installation:

Backend Server Installation:

Install MediaPipe Python:
Copy code
pip install mediapipe
Install OpenCV Python:
Copy code
pip install opencv-python
Navigate to the backend directory and install other requirements:
Copy code
pip install -r requirements.txt
Download the pre-trained generator model for the COCO dataset and place it into backend/checkpoints/coco_pretrained/.
Unity3D Installation:

Download and install UnityHub.
Add a new license in UnityHub and register it.
Install a Unity Editor inside UnityHub (LTS versions and a version higher than 2020.3.25f1 are recommended).
In the Unity project settings, allow HTTP connections in the player settings.
Usage:

Run the backend server at the backend directory with the following command:
Copy code
python server.py
Run the Unity project and open the main scene at Assets\Scenes\MainScene.unity.
Test the program by uploading videos to the backend from the Unity project (You can test the application by selecting provided animations from the right-side menu).
Adding New 3D Characters:

Find a 3D character model from the Unity asset store or download a free one.
Set the rig to humanoid in the character settings.
Drag and drop your 3D character model to CharacterChooser/CharacterSlideshow/Parent object in Unity main Scene.
Add BlendShapeController and QualityData components to the character object in the scene.
Set BlendShapeController values and add character SkinnedMeshRenderer component to BlendShapeController component.
Add the character to the nodes property of CharacterSlideshow Object.
Run the application and select your character for rendering animation.
Features:

Making full body animation.
Animating multiple blendShapes on 3D character (up to 40 blendshape animations are supported currently).
Supporting any 3D models with Humanoid T-Pose rig.
Exporting animation in a video file.
Saving animation data and re-rendering it for future usage.
Filtering MediaPipe outputs to detect and remove noises and better smoothness (Low Pass Filtering is used currently).
Animating the character's face in great detail.
Training a regression model to generate Blendmesh weights by feeding the output data of MediaPipe FaceMesh (468 points).
Using StyleGan techniques to replace the whole character face mesh.
Automatic rigging for 3D models without a humanoid rig (Using deep neural network models like RigNet).
Generating a complete character mesh automatically using models like PIFuHD (in progress!).
Animating the 3D character's mouth in great detail using audio signal or natural language processing methods.
Generating a complete environment in 3D.
