# KAIMyEntity-C

KAIMyEntity allows you to render 3D models of MikuMikuDance instead of default entities.  

## How to use

### What you need to prepare

#### Indispensable

* [This mod](https://github.com/Gengorou-C/KAIMyEntity-C/releases)
* 3D model file (PMX or PMD)
* [KAIMyEntitySaba.dll](https://github.com/Gengorou-C/KAIMyEntitySaba/releases/tag/20221215)
* [MMDShader.fsh, MMDShader.vsh](https://github.com/Gengorou-C/KAIMyEntity-C/releases/tag/requiredFiles)

#### Almost indispensable

* [Default VMD files](https://github.com/Gengorou-C/KAIMyEntity-C/releases/tag/requiredFiles)
* [lightMap.png](https://github.com/Gengorou-C/KAIMyEntity-C/releases/tag/requiredFiles)

#### Recommended

* Dedicated VMD files for each 3D model
* [model.properties](https://github.com/Gengorou-C/KAIMyEntity-C/releases/tag/requiredFiles)

### Installation

1. Download the appropriate .jar file and place it in the `mods` folder.  
2. Run minecraft.  
3. If the KAIMyEntity folder doesn't exist in the game's directory, this mod will create it by downloading a ZIP file and extracting it on the game's root folder.
4. If the KAIMyEntitySaba.dll file doesn't exist in the game's directory, it will be downloaded on the game's root folder.  
5. Open the KAIMyEntity folder and then copy and paste the EntityPlayer folder.  
6. Rename the copied EntityPlayer folder to `EntityPlayer_[username]` (e.g.) "EntityPlayer_Gengorou-C"  
7. Place the 3D model files inside the `EntityPlayer_[username]` folder.  
8. Rename the 3D model file to `model.pmx` or `model.pmd`, depending on the model's original format.
9. Start the game, select world and start playing.

### Example of the directory tree

```bash
.
├── config
├── KAIMyEntity
│   ├── DefaultAnim
│   │   └── Default VMD files
│   ├── EntityPlayer
│   │   ├── Texture files
│   │   ├── Dedicated VMD files
│   │   ├── lightMap.png
│   │   ├── model.properties
│   │   └── model.pmx (or model.pmd)
│   ├── EntityPlayer_(Player Name)
│   │   ├── Texture files
│   │   ├── Dedicated VMD files
│   │   ├── lightMap.png
│   │   ├── model.properties
│   │   └── model.pmx (or model.pmd)
│   ├── (entity ID) (e.g. minecraft.horse)
│   │   ├── Texture files
│   │   ├── Dedicated VMD files
│   │   ├── lightMap.png
│   │   └── model.pmx (or model.pmd)
│   └── Shader
│       ├── MMDShader.fsh
│       └── MMDShader.vsh
├── logs
├── mods
│   └──KAIMyEntityC.jar
├── saves
├── shaderpacks
├── KAIMyEntitySaba.dll
└── ...
```

## Motion list

### Player

```
EntityPlayer_[username]
├── idle.vmd
├── walk.vmd
├── sprint.vmd
├── sneak.vmd
├── swim.vmd
├── elytraFly.vmd
├── onClimbable.vmd
├── onClimbableUp.vmd
├── onClimbableDown.vmd
├── crawl.vmd
├── lieDown.vmd
├── sleep.vmd
├── ride.vmd
├── onHorse.vmd
├── swingRight.vmd
├── swingLeft.vmd
├── die.vmd
│
├── custom_1.vmd
├── custom_2.vmd
├── custom_3.vmd
├── custom_4.vmd
│
├── itemActive_[itemName]_[Left/Right]_[using/swinging].vmd
│   (e.g.)
│       itemActive_minecraft.shield_Left_using.vmd
│       itemActive_minecraft.iron_sword_Right_swinging.vmd
│
├── model.pmx (or model.pmd)
├── model.properties
└── lightMap.png
```

### Entity

```
EntityPlayer_[entityName]
├── idle.vmd
├── walk.vmd
├── swim.vmd
├── ridden.vmd
├── driven.vmd
```

## Others

* If you want to change the model size or item angle, you can edit them in the `model.properties` file.  