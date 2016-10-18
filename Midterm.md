# Midterm Game Programming

## Introduction and Game Engine

### Write at least two benefits that you gain when using a game engine for your game development. 
  - Reusable software components
  - most of the game engine are  Cross platform where u have to do little work to port ur game.
  - memory management, asset loading, lighting (in complex engines), etc has all been designed and tested thoroughly 
  
### What do you mean by “Platform-independent” game engine?
  - you can create a game and with minimal changes to code you can deploy your game in multiple platform

### Write three types of game engines. To which game type does Unity belong?
  - Roll-your-own game engines (lowest level)
  - Mostly-ready game engines (mid level). 
  - Point-and-click engines (highest level). Unity belongs to this type.
 
### Write at least three names of Open Source Game engines.
  - Crystal Space.
  - Delta3D.
  - Panda 3D
  - Wolfenstein 3D engine
  
## Unity game engine questions

### Write at least two distinct features of Unity game engine compared to other Game Engines.
  - Unity supports Animation with models better than any other game engine
  - cross platform is much simpler.
  - the interface for user are much simpler that can be learnt at ease.
  - one click deployment
  - Asset store is one of the big plus for unity that makes Unity more distinct

### Define “Assets”. Give examples of art assets ?
  - all the content (models, animations, sounds, AI, and physics) which are called 'assets‘

### prefabs? 
  - Unity has a Prefab asset type that allows you to store a GameObject object complete with components and properties. 
  - The prefab acts as a template from which you can create new object instances in the scene. 
  - Any edits made to a prefab asset are immediately reflected in all instances produced from it but you can also override components and settings for each instance individually.
 
### HUD ? 
  - heads up display 
  - it is a 2d View mostly helpfull to build our GUI.

### NPC
  - Non Player Character
  - it means any character that player cant control. eg: AI that wanders around and has its own behavior.

### NavMesh Baking
  - The process of creating a NavMesh from the level geometry is called NavMesh Baking. 
  - The process collects the Render Meshes and Terrains of all Game Objects which are marked as Navigation Static, and then processes them to create a navigation mesh that approximates the walkable surfaces of the level.

### What are three types of lights in Unity? Which light is like the Sun in real world?
  - point lights 
  - spot lights
  - directional lights (Sun in real world)
  - emisive lights
  - area lights
  - ambient light

### In the following code segment, what does [SerializeField] attribute do?
    [SerializeField] private float speed;
   - this means the speed variable is private in its script but serilize field enables us to manipulate the speed from the inspector. 

### What does the code segment do?
    using UnityEngine;
    using System.Collections;
    public class Unknown : MonoBehaviour {
    public float speed = 3.0f;
    void Update() {
    transform.Rotate(0, speed, 0);
    }
    }
  - if this script is attached to an cube it will rotate the cube to its own y-axis.

### What does the code segment do?
      transform.Rotate(0, speed, 0);
      transform.Rotate(0, speed, 0, Space.World);
  - adding Space.World will rotate the object to World y axis not the object y-axis.
  
### What is raycasting? Describe when (for what purpose) you use it for your homework?
   - it means casting a ray from the given origin to the specified direction with specified distance. the ray will collect all the information about the collider object. ray can be casted from the origin to the mentioned direction infinitly.
   - In our homework we used it to cast a ray from player character to infinite distance to get the information on what we are shooting at.
   
### Coroutine
  - A coroutine is like a function that has the ability to pause execution and return control to Unity but then to continue where it left off on the following frame
