<h1 id="Top">切石机增强 Cutter Plus</h1>

- 作者 Author: 莫yis
- 版本 Version: 2.8.2
- 支持版本 Supported version: 1.14.4 ~ 1.17.1
- Github: https://github.com/Mo-yis/CutterPlus
- Gitee: https://gitee.com/Mo-yis/CutterPlus

<h2>献辞 Dedication</h2>

    谨将此数据包, 献给所有努力生存的方块人！

    This datapack is dedicated to all those who strive to survive!

<h2 id="Contents">目录 Contents</h2>
<ol>
    <li><a href="#Explain">说明 Explain</a></li>
    <li>
        <a href="#Features">特性 Features</a>
        <ol>
            <li>
            <a href="#Vanilla-Support">原版支持 Vanilla Support</a>
                <ol>
                    <li><a href="#Wooden-Crafting-Tree">木制物品加工图 Wooden Crafting Tree</a></li>
                    <li><a href="#Stony-Crafting-Tree">石质物品加工图 Stony Crafting Tree</a></li>
                    <li><a href="#Coppery-Crafting-Tree">铜质物品加工图 Coppery Crafting Tree</a></li>
                </ol>
            </li>
            <li>
            <a href="#tconstruct">匠魂支持 Tinkers' Construct Support</a>
                <ol>
                    <li><a href="#Tinkers-General-Items">Tinkers' General Items</a></li>
                    <li><a href="#Tinkers-Smeltery">Tinkers' Smeltery</a></li>
                    <li><a href="#Tinkers-World">Tinkers' World</a></li>
                    <li><a href="#Mod-Compatibility">模组兼容 Mod Compatibility</a></li>
                </ol>
            </li>
        </ol>
    </li>
    <li><a href="#Update">更新内容 Update</a></li>
    <li><a href="#Update-Plan">计划更新 Update Plan</a></li>
    <li><a href="#Usage">使用方式 Usage</a></li>
    <li><a href="#Warming">注意 Warming</a></li>
</ol>

<h2 id="Explain">说明 Explain</h2>

- 一个轻量级数据包，仅使用一个加工工具，方便加工。
- 在不破坏原版游戏平衡的情况下添加大量切石机的工作配方。
- 你甚至可以用切石机切木头！ Emmm... 在生活中是可以的。
- 从版本 “2.4” 开始，支持模组《匠魂 - 1.16.5》。
- 分支选择：
    - main: 默认版（含forge）
    - vanilla: 原版
    - dev-: 开发版，请勿选择

<br>

- A lightweight datapack that uses only one processing tool to facilitate processing.
- Blocks that need to be burned cannot be obtained from stone-cutter, such as smooth stones.
- You can even cut wood with a stone-cutter! Emmm... It's OK in life.
- Starting from version "2.4", the Mod "Tinkers' Construct - 1.16.5" is supported.
- Select branch:
    - main: Default version (including forge version).
    - vanilla: None mods.
    - dev-: Development version, please do not select.

<h2 id="Features">特性 Features</h2>

- 要经过烧炼才能获得的方块无法从切石机获得，如平滑石头。
- 苔石和苔石砖是由圆石和石砖加工而来，故不能相互转化。
- 切石机只能加工固态物品和没有NBT标签的物品（从设计的角度上来看）。
- 使用Forge的通用矿物词典标签。
- 未加载的配方使用 “空气” 填充，保证多个Mod之间兼容。

<br>

- Blocks that can only be obtained by burning cannot be obtained from a stone cutter, such as the smooth_stones.
- The mossy_cobblestone and the mossy_stone_bricks are processed from the cobblestone and the stone_bricks, so they can not be transformed into each other.
- The stone-cutter can only process solid articles and articles without NBT label.(From the design point of view.)
- Use forge's generic mineral dictionary label.
- Unloaded recipes are filled with "air" to ensure compatibility between multiple mods.

<a href="#Contents">回到目录 Back to contents</a>
<h3 id="Vanilla-Support">原版支持 Vanilla Support</h3>
<h4 id="Wooden-Crafting-Tree">木制物品加工图 Wooden Crafting Tree</h4>

```
------------------------------------------------------------------
木头种类 wooden_type
    |-- 原木 log (菌柄 stem)
        |-- 木头 wood (菌核 hyphae)
        |-- 木板 planks [4]
        |-- 去皮原木 stripped_log (去皮菌柄 stripped_stem)
            |-- 去皮木头 stripped_wood (去皮菌核 stripped_hyphae)
            |-- 木板 planks [4]
    |-- 木头 wood (菌核 hyphae)
        |-- 木板 planks [4]
        |-- 去皮木头 stripped_wood (去皮菌核 stripped_hyphae)
            |-- 木板 planks [4]
    |-- 木板 planks
        |-- 栅栏 fence
        |-- 台阶 slab [2]
        |-- 按钮 button
        |-- 楼梯 stairs
            |-- 台阶 slab
------------------------------------------------------------------
(物品 items ------->> 木棍 stick [1])
木台阶 wooden_slab                 木楼梯 wooden_stairs
树苗 sapling                       树叶 leaves
竹子 bamboo                        脚手架 scaffolding
枯萎的灌木 dead_bush

(物品 items ------->> 木棍 stick [2])
木栅栏 wooden_fence                梯子 ladder
织布机 loom                        木板 planks
木压力板 wooden_pressure_plate      画 painting
物品展示框 item_frame

(物品 items ------->> 木棍 stick [4])
木门 wooden_door                   木栅栏门 wooden_fence_gate
木告示牌 wooden_sign               木活板门 wooden_trapdoor
讲台 lectern                       制图台 cartography_table
制箭台 fletching_table             锻造台 smithing_table
工作台 crafting_table              (灵魂)营火 (soul)campfire
床 beds

(物品 items ------->> 木棍 stick [6])
船 boat                           堆肥桶 composter
盔甲架 armor_stand                 木桶 barrel
蜂箱 beehive                       书架 bookshelf

(物品 items ------->> 木棍 stick [8])
木头 wood (菌核 hyphae)            唱片机 jukebox
箱子 chest                         陷阱箱 trapped_chest
音符盒 note_block                  原木 log (菌柄 stem)
去皮原木 stripped_log (去皮菌柄 stripped_stem)
去皮木头 stripped_wood (去皮菌核 stripped_hyphae)
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Stony-Crafting-Tree">石质物品加工图 Stony Crafting Tree</h4>

```
------------------------------------------------------------------
- 相互转化

(方块)
紫珀块 <=========>  紫珀柱
花岗岩 <=========>  磨制花岗岩
闪长岩 <=========>  磨制闪长岩
安山岩 <=========>  磨制安山岩
玄武岩 <=========>  磨制玄武岩
末地石 <=========>  末地石砖
下界砖块 <=======>  錾制下界砖块
基岩 <===========>  命令方块 <=====>  结构方块
石头 <===========>  石砖 <========>  錾制石砖
砂岩 <===========>  錾制砂岩 <=====>  切制砂岩
红砂岩 <=========>  錾制红砂岩 <====>  切制红砂岩
黑石 <===========>  磨制黑石 <=====>  磨制黑石砖 <====> 錾制磨制黑石砖
石英块 <=========>  石英砖 <=======>  錾制石英块 <====> 石英柱
深板岩圆石 <==> 錾制深板岩 <==> 磨制深板岩 <==> 深板岩砖 <==> 深板岩瓦

(台阶 / 楼梯)
石头 <========>  石砖
花岗岩 <======>  磨制花岗岩
闪长岩 <======>  磨制闪长岩
安山岩 <======>  磨制安山岩
黑石 <========>  磨制黑石 <===>  磨制黑石砖
深板岩圆石 <===>  錾制深板岩 <==>  磨制深板岩 <==> 深板岩砖 <==> 深板岩瓦

(墙)
黑石墙 <=====>  磨制黑石墙 <==>  磨制黑石砖墙

- 单向转化

楼梯 ----------->>  台阶
玻璃(染色) ------>>  玻璃板(染色) [3]
滴水石块 -------->>  滴水石锥
石头 ----------->>  石头按钮
黑石 ----------->>  磨制黑石按钮  <<----- 磨制黑石
紫水晶块 -------->>  紫水晶碎片
紫水晶簇 -------->>  紫水晶碎片 [3]
蓝冰 ----------->>  浮冰 ------------>>  冰
石英块 ---------->>  下界石英
下界砖台阶 ------>>  下界砖 [2]   <<----- 下界砖楼梯
下界砖块 -------->>  下界砖 [4]
砖台阶 ---------->>  红砖 [2]   <<------- 砖楼梯
砖块 ----------->>  红砖 [4]
铁块 ----------->>  铁锭 [9] -------->> 铁粒 [9]
金块 ----------->>  金锭 [9] -------->> 金粒[9]
下界合金块 ------>>  下界合金锭 [9]
钻石块 ---------->>  钻石 [9]
绿宝石块 -------->>  绿宝石 [9]
青金石块 -------->>  青金石 [9]
海晶石砖台阶 ----->>  海晶石台阶
海晶石砖楼梯 ----->>  海晶石楼梯
海晶石砖 -------->>  海晶石 ---->>  海晶石碎片 <<------ 海晶灯
------------------------------------------------------------------
- Exchange

(Block)
purpur_block <=====>  purpur_pillar
granite <==========>  polished_granite
diorite <==========>  polished_diorite
andesite <=========>  polished_andesite
basalt <===========>  polished_basalt
end_stone <========>  end_stone_bricks
nether_bricks <====>  chiseled_nether_bricks
bedrock <==========>  command_block <==========> structure_block
stone <============>  stone_bricks <==> chiseled_stone_bricks
sandstone <========>  chiseled_sandstone<======> cut_sandstone
red_sandstone <====>  chiseled_red_sandstone<==> cut_red_sandstone
blackstone <=======>  polished_blackstone<======>
    polished_blackstone_bricks <==> chiseled_polished_blackstone
quartz_block <=====>  quartz_bricks <============>
    chiseled_quartz_block <==========>  quartz_pillar
cobbled_deepslate <==> chiseled_deepslate <======>
    polished_deepslate <==> deepslate_bricks <==> deepslate_tiles

(Slab / stairs)
stone <=======>  stone_brick
granite <=====>  polished_granite
diorite <=====>  polished_diorite
andesite <====>  polished_andesite
blackstone <==>  polished_blackstone <==> polished_blackstone_brick
cobbled_deepslate <=====> chiseled_deepslate <=====>
    polished_deepslate <===> deepslate_bricks <===> deepslate_tiles

(wall)
blackstone_wall <=====> polished_blackstone_wall
    <====> polished_blackstone_brick_wall

- Transform to

stairs ---------------->>  slab
glass(stained) -------->>  glass_pane(stained) [3]
dripstone_block ------->>  pointed_dripstone
stone ----------------->>  stone_button
blackstone ------------>>  polished_blackstone_button
    <<------- polished_blackstone
amethyst_block -------->>  amethyst_shard
amethyst_cluster ------>>  amethyst_shard [3]
blue_ice -------------->>  packed_ice -------->> ice
quartz_block ---------->>  quartz
nether_brick_slab ----->>  nether_brick [2] <<-- nether_brick_stairs
nether_bricks --------->>  nether_brick [4]
brick_slab ------------>>  brick [2]  <----- brick_stairs
bricks ---------------->>  brick [4]
iron_block ------------>>  iron_ingot [9] ---->>  iron_nugget [9]
gold_block ------------>>  gold_ingot [9] ---->>  gold_nugget [9]
netherite_block ------->>  netherite_ingot [9]
diamond_block --------->>  diamond [9]
emerald_block --------->>  emerald [9]
lapis_block ----------->>  lapis_lazuli [9]
prismarine_brick_slab --->>  prismarine_slab
prismarine_brick_stairs ->>  prismarine_stairs
prismarine_bricks ---->>  prismarine --------->>
    prismarine_shard <<------- sea_lantern
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Coppery-Crafting-Tree">铜质物品加工图 Coppery Crafting Tree</h4>

```
------------------------------------------------------------------
(先) 打蜡的 -->>  未打蜡的
(后) 氧化的 -->>  锈蚀的 -->> 斑驳的 -->> 新的
块状的 <======>  切制的
楼梯 -->>  台阶 ------>> 铜锭 [4]
楼梯 -->>  铜锭 [4]
铜块 -->>  铜锭 [9] <<---- 切制铜块

(first) waxed ------>>  unwaxed
(second) oxidized -->>  weathered -->> exposed -->> new
block <=========>  cut
stairs ------------->>  slab ------>> copper_ingot [4]
stairs ------------->>  copper_ingot [4]
copper_block ------->>  copper_ingot [4] <<---- cut_copper
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="tconstruct">匠魂支持 Tinkers' Construct Support</h3>
<h4 id="Tinkers-General-Items">Tinkers' General Items</h4>

```
------------------------------------------------------------------
mud_bricks -->>  mud_bricks_stairs --->> mud_bricks_slab
mud_bricks -->>  mud_bricks_slab [2]
lavawood ---->>  lavawood_stairs ----->> lavawood_slab
lavawood ---->>  lava_slab [2]
blazewood --->>  blazewood_stairs ---->> blazewood_slab
blazewood --->>  blazewood_slab [2]
nahuatl ----->>  nahuatl_stairs ------>> nahuatl_slab
nahuatl ----->>  nahuatl_slab [2]
nahuatl ----->>  nahuatl_fence

(glass)
clear_glass -->> clear_glass_pane [3]
soul_glass -->> soul_glass_pane [3]
clear_stained_glass -->> clear_stained_glass_pane [3]

(block -->> ingot [9] -->> nugget [9])
copper              cobalt
slimesteet          tinkers_bronze
rose_gold           pig_iron
queens_slime        manyullyn
hepatizon
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Tinkers-Smeltery">Tinkers' Smeltery</h4>

```
------------------------------------------------------------------
seared_stone <=====> seared_bricks <=======> 
    seared_fancy_bricks <==> seared_triangle_bricks

seared_bricks_stairs -->>  seared_brick_slab
seared_bricks --------->>  seared_brick [4]
seared_bricks_stairs -->>  seared_brick [2] <<-- seared_bricks_slab
seared_glass ---------->>  seared_glass_pane [3]

scorched_bricks <==> chiseled_scorched_bricks <==>
    polished_scorched_stone <==> scorched_stone <==> scorched_road
scorched_bricks_slab <==> scorched_road_slab
scorched_bricks_stairs <==> scorched_road_stairs

scorched_bricks --------->>  scorched_bricks_fence
scorched_bricks_stairs -->>  scorched_bricks_slab
scorched_road_stairs ---->>  scorched_road_slab
scorched_bricks --------->>  scorched_brick [4]
scorched_bricks_stairs -->>  scorched_brick [2] <<-- scorched_bricks_slab
scorched_glass ---------->>  scorched_glass_pane [3]
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Tinkers-World">Tinkers' World</h4>

```
------------------------------------------------------------------
木头种类 wooden_type
    |-- 原木 log (菌柄 stem)
        |-- 木头 wood (菌核 hyphae)
        |-- 木板 planks [4]
        |-- 去皮原木 stripped_log (去皮菌柄 stripped_stem)
            |-- 去皮木头 stripped_wood (去皮菌核 stripped_hyphae)
            |-- 木板 planks [4]
    |-- 木头 wood (菌核 hyphae)
        |-- 木板 planks [4]
        |-- 去皮木头 stripped_wood (去皮菌核 stripped_hyphae)
            |-- 木板 planks [4]
    |-- 木板 planks
        |-- 栅栏 fence
        |-- 台阶 slab [2]
        |-- 按钮 button
        |-- 楼梯 stairs
            |-- 台阶 slab

wooden_sign -->> stick [4] <<-- wooden_fence_gate
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility">模组兼容 Mod Compatibility</h4>

```
------------------------------------------------------------------
(item swap)
forge:copper(ingot/nugget/ore/block)

netherite_ingot(minecraft) -->> netherite_nugget
obsidian(minecraft) -->> obsidian_pane
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h2 id="Update">更新内容 Update</h2>

- 更新 README。

<h2 id="Update-Plan">计划更新 Update Plan</h2>

- 支持机械动力。
- 支持暮色森林。
- 支持更多1.16.5的开源模组。

<a href="#Contents">回到目录 Back to contents</a>
<h2 id="Usage">使用方式 Usage</h2>

- 首先，请在左上角选择需要下载的分支，默认 “**main**” 分支。
- Github: 右上角点击**绿色**的 "**Code**" 再点击 "**Download ZIP**"。
- Gitee: 右上角点击**橙色**的 "**克隆/下载**" 再点击 "**下载ZIP**"。

<br>

- 如果你打算将数据包放入存档中，请解压在 ".minecraft\\saves\\(存档名称)\\datapacks\\" 目录下。
- 如果你正准备新建世界，请将解压出的文件夹添加到游戏中。
- 如果你打算加载到已经启动的游戏或服务器中，请在后台或以3级操作员身份键入 "/reload" 以加载数据包。
- 相关疑问请查询 Minecraft Wiki。

<br>

- First, select the branch to download in the upper left corner. The default branch is "**main**".
- Github: Click the **green** "**Code**" in the upper right corner and then click "**Download ZIP**".
- If you plan to put the datapack into the archive, please unzip it in the ".minecraft\\saves\\(save name)\\datapacks\\" directory.
- If you are preparing to create a new world, please add the extracted folder to the game.
- If you plan to load into a game or server that has already started, please type "/reload" from the console or as a level 3 operator.
- For questions, please check the Minecraft Wiki.

<a href="#Contents">回到目录 Back to contents</a>
<h2 id="Warming">注意 Warming</h2>

- 与Mod不同，数据包仅对单个世界有效。
- 数据包兼容一定范围内的版本，但是不会针对旧版本进行维护。
- 请勿添加功能类似或相同的数据包。
- 合成配方可以通过JSON文件修改，但不推荐这么做。
- 当数据包成功加载时，游戏中会提示 "[ 数据包名称 ] Loading Successful !"。
- 版本低于1.15.2无法显示提示信息，请以管理员身份键入命令 "/datapack list" 查看数据包信息。

<br>

- Unlike Mod, datapack are only valid for a single world.
- Datapack is compatible with a certain range of versions, but it will not be maintained for the old version.
- Do not add datapack with similar or identical functions.
- Synthetic recipes can be modified through JSON files, but this is not recommended.
- When the datapack is successfully loaded, the game will prompt "[ datapack name ] Loading Successful !".
- The prompt message cannot be displayed in versions lower than "1.15.2". Please type the command "/datapack list" as an administrator to view the datapack information.

<a href="#Contents">回到目录 Back to contents</a>
