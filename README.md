# 切石机增强 Cutter Plus

- 数据包版本 Datapack Version: v3.0.13
- 支持版本 Supported version: 1.14.4 ~ 1.18.1
- Github: https://github.com/Mo-yis/CutterPlus

## 说明 Explain

- 一个轻量级数据包，添加了大量切石机的工作配方。
- 你甚至可以用切石机切木头！ Emmm... 在生活中是可以的。
- 从版本 “2.4” 开始，使用 “Forge” 的通用矿物词典标签。
- 未加载的配方使用 “空气” 填充，保证多个模组之间兼容。
- 如果觉得空气配方碍眼，可以将没有的模组对应的以 “support” 开头的文件夹删除：
```
1. minecraft --------- 《Minecraft》是最早支持的内容。
2. tconstruct -------- 《匠魂 - 1.16.5》从版本 “2.4” 开始支持。
3. create ------------ 《机械动力 - 1.16.5》从版本 “2.9” 开始支持。
4. twilightforest ---- 《暮色森林 - 1.16.5》从版本 “2.10” 开始支持。
5. biomesoplenty ----- 《超多生物群系 - 1.16.5》从版本 “2.11” 开始支持。
6. bayou_blues ------- 《长沼蓝调 - 1.16.5》从版本 “2.12” 开始支持。
7. autumnity --------- 《秋原 - 1.16.5》从版本 “2.13” 开始支持。
8. quark ------------- 《夸克 - 1.16.5》从版本 “2.14” 开始支持。
```

<br />

- A lightweight data package that adds a large number of working formulas for stone-cutter.
- You can even cut wood with a stone-cutter! Emmm... It's OK in life.
- Starting with version "2.4", use the general mineral dictionary label of "Forge".
- Unloaded recipes are filled with "air" to ensure compatibility between multiple mods.
- If you think the air recipe is eye-catching, you can delete the folder starting with "support" corresponding to the uninstalled mod:
```
1. minecraft --------- "Minecraft" was the first supported content.
2. tconstruct -------- "Tinkers' Construct - 1.16.5" is supported from version "2.4".
3. create ------------ "Create - 1.16.5" is supported from version "2.9".
4. twilightforest ---- "The Twilight Forest - 1.16.5" is supported from version "2.10".
5. biomesoplenty ----- "Biomes O' Plenty - 1.16.5" is supported from version "2.11".
6. bayou_blues ------- "Bayou Blues - 1.16.5" is supported from version "2.12".
7. autumnity --------- "Autumnity - 1.16.5" is supported from version "2.13".
8. quark ------------- "Quark - 1.16.5" is supported from version "2.14".
```

## 特性 Features

- 要经过烧炼才能获得的方块无法从切石机获得，如平滑石头。
- 切石机只能加工固态物品和没有NBT标签的物品（从设计的角度上来看）。
- 同一类的方块（材质不同）之间可以相互转化（方块，楼梯，台阶，墙）。
- 苔石和苔石砖是由圆石和石砖加工而来，故不能相互转化。其他情况类似。
- 楼梯可以加工成对应的台阶。
- 请在 WIKI 页面查看详细配方: https://github.com/Mo-yis/CutterPlus/wiki

<br />

- Blocks that can only be obtained by burning cannot be obtained from a stone cutter, such as the smooth_stones.
- The stone-cutter can only process solid articles and articles without NBT label.(From the design point of view.)
- Blocks of the same type (with different appearance) can be transformed into each other (block, stair, slab, wall).
- The mossy_cobblestone and the mossy_stone_bricks are processed from the cobblestone and the stone_bricks, so they can not be transformed into each other.Other situations are similar.
- Stairs can be processed into corresponding slab.
- Please check the detailed Recipe on WIKI page: https://github.com/Mo-yis/CutterPlus/wiki

## 计划更新 Update Plan

- 更新模组内容支持
- 添加更多模组间兼容性配方
- 调整文件夹目录、规范文件命名
- 支持更多1.16.5的模组

## 使用方式 Usage

- Github: 右上角点击**绿色**的 "**Code**" 再点击 "**Download ZIP**"。
- 如果你打算将数据包放入存档中，请解压在 ".minecraft \\ saves \\ (存档名称) \\ datapacks \\ " 目录下。
- 如果你正准备新建世界，请将解压出的文件夹添加到游戏中。
- 如果你打算加载到已经启动的游戏或服务器中，请在后台或以3级操作员身份键入 "/reload" 以加载数据包。
- 相关疑问请查询 Minecraft Wiki。

<br />

- Github: Click the **green** "**Code**" in the upper right corner and then click "**Download ZIP**".
- If you want to put the datapack into the archive, please unzip it in the ".minecraft \\ saves \\ (save name) \\ datapacks \\ " directory.
- If you are preparing to create a new world, please add the extracted folder to the game.
- If you want to load into a game or server that has already started, please type "/reload" from the console or as a level 3 operator.
- For questions, please check the Minecraft Wiki.

## 注意 Warming

- 与模组不同，数据包仅对单个世界有效。但是有些 MOD 可以实现在多个世界中共享数据包。
- 数据包兼容一定范围内的版本，但是不会针对旧版本进行维护。
- 请勿添加功能类似或相同的数据包。
- 当数据包成功加载时，游戏中会提示 "[ 数据包名称 ] Loading Successful !"。
- 版本低于1.15.2无法显示提示信息，请以管理员身份键入命令 "/datapack list" 查看数据包信息。

<br />

- Unlike Mod, datapack are only valid for a single world. However, some mods can share datapacket in multiple worlds.
- Datapack is compatible with a certain range of versions, but it will not be maintained for the old version.
- Do not add datapack with similar or identical functions.
- When the datapack is successfully loaded, the game will prompt "[ datapack name ] Loading Successful !".
- The prompt message cannot be displayed in versions lower than "1.15.2". Please type the command "/datapack list" as an administrator to view the datapack information.
- Extremely sorry for my bad English.
