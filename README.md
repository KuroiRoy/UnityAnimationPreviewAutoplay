# UnityAnimationPreviewAutoplay
Enhances animation browsing experience in the Unity editor by forcing the preview window to autoplay the animation clip.

## Instructions
Place the script inside an Editor folder somewhere in your project's Assets. 

## How it works
The script checks every editor update if the selected object shown in the inspector has changed. Then it checks if the selected object is an animation or a gameobject with an animation. After an animation is found there is a delay of a few frames before the inspector shows the animation preview. Once the script sees the animation preview it forces the animation time controls to start playing the animation.

Reflection is used to gain access to the fields and properties of the animation preview and to set the "playing" value.
