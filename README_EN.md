# KAIMyEntity-C

KAIMyEntity allows you to render 3D MikuMikuDance (MMD) models instead of the default Minecraft entities.

I am not a professional programmer, and I cannot guarantee that this mod will be completely free of bugs or provide official support.

## How to Use

### Requirements

#### Essential

* [This mod](https://github.com/Gengorou-C/KAIMyEntity-C/releases)
* 3D model file (PMX or PMD)
* [KAIMyEntitySaba.dll](https://github.com/Gengorou-C/KAIMyEntitySaba/releases/tag/20221215)
* [MMDShader.fsh, MMDShader.vsh](https://github.com/Gengorou-C/KAIMyEntity-C/releases/tag/requiredFiles)

#### Highly Recommended

* [Default VMD files](https://github.com/Gengorou-C/KAIMyEntity-C/releases/tag/requiredFiles)
* [lightMap.png](https://github.com/Gengorou-C/KAIMyEntity-C/releases/tag/requiredFiles)

#### Optional but Recommended

* Dedicated VMD files for each 3D model
* [model.properties](https://github.com/Gengorou-C/KAIMyEntity-C/releases/tag/requiredFiles)

---

### Installation

1. Download the appropriate `.jar` file and place it in the `mods` folder.
2. Launch Minecraft.
3. If the `KAIMyEntity` folder does not exist in the game directory, the mod will automatically download and extract it from a ZIP file.
4. If `KAIMyEntitySaba.dll` is missing from the game directory, it will be downloaded automatically.
5. Open the `KAIMyEntity` folder, then copy and paste the `EntityPlayer` folder.
6. Rename the copied `EntityPlayer` folder to `EntityPlayer_(YourName)` (e.g., `EntityPlayer_Gengorou-C`).
7. Place your 3D model files in the `EntityPlayer_(YourName)` folder.
8. Rename your 3D model file to `model.pmx` (or `model.pmd`).
9. Select a world and start the game.

---

### Example Directory Tree

```bash
.
├── config
├── KAIMyEntity
│   ├── DefaultAnim
│   │   └── default VMD files
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
│   ├── (entity ID) (e.g., minecraft.horse)
│   │   ├── Texture files
│   │   ├── Dedicated VMD files
│   │   ├── lightMap.png
│   │   └── model.pmx (or model.pmd)
│   └── Shader
│       ├── MMDShader.fsh
│       └── MMDShader.vsh
├── logs
├── mods
│   └── KAIMyEntityC.jar
├── saves
├── shaderpacks
├── KAIMyEntitySaba.dll
└── ...
```

---

## Motion List

### Player Motions

* idle.vmd
* walk.vmd
* sprint.vmd
* sneak.vmd
* swingRight.vmd
* swingLeft.vmd
* elytraFly.vmd
* swim.vmd
* onClimbable.vmd
* onClimbableUp.vmd
* onClimbableDown.vmd
* sleep.vmd
* ride.vmd
* die.vmd
* custom\_\[1-4].vmd
* itemActive\_\[itemName]*\[Left or Right]*\[using or swinging].vmd

  * Example: `itemActive_minecraft.shield_Left_using.vmd`
  * Dedicated motion for specific items
* onHorse.vmd
* crawl.vmd
* lieDown.vmd

### Entity Motions

* idle.vmd
* walk.vmd
* swim.vmd
* ridden.vmd
* driven.vmd

---

## Other Notes

* To change the model size or adjust the item angle, edit the `model.properties` file.

---

If you want, I can also rewrite this into a **fully polished GitHub README.md** format so it looks cleaner and more professional on the repository page.
Do you want me to prepare that?
