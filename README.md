# VRay Shader Creator

This tool helps create a VRay Shader automatically by specifying a folder that has the texture maps. 

# Installation

1. Download VRayShaderCreator.mzp based on your 3DS Max version
2. Drag and drop VRayShaderCreator.mzp into the 3DS Max Viewport.
3. You will see a "Installed~" message and an orange icon will appear in the toolbar.


![Installation Toolbar](https://i.imgur.com/k0mc790.jpeg)

# Usage

1. Click the orange icon and you will see the Vray Shader Creator window. 

![Installation Toolbar](https://i.imgur.com/faSo8qL.jpeg)

2. Provide a location to a folder with the textures in it.

> [!NOTE]
> This script only works with the following naming convention.
```
Diffuse/Albedo - BaseColor.<UDIM>.exr
Normal - Normal.<UDIM>.exr
Bump - Height.<UDIM>.exr
Metalness - Metallic.<UDIM>.exr
Specular Roughness - Roughness.<UDIM>.exr
```

> [!IMPORTANT]
> **All textures must be in .exr format.**

I have also added an export preset for Substance Painter that will export all the textures with correct naming conventions. 

*Later script versions will allow to choose from other extensions.*

3. Check/Uncheck the texture types based on the shader you want to create and press Create Shader. The output window will display an echo of all the steps. If all goes well, there will be a new VRay Mtl shader created in the first slot of the Material Editor.

![Installation Toolbar](https://i.imgur.com/4GuA4v5.jpeg)

> [!WARNING]
> If you have a texture type checked and the texture maps are not in the folder, the tool will abort the shader creation process. 

For now, the tool only creates the shader in the Compact Material Editor. You can access the same Vray MTL shader in the Slate Material Editor by going to the Sample Slots and drag-dropping the shader into the graph editor. 

![Installation Toolbar](https://i.imgur.com/FfJ59cf.jpeg)

4. Apply the shader on to your mesh!

![Installation Toolbar](https://i.imgur.com/crgxDus.jpeg)
