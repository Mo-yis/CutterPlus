<h1 id="Top">切石机增强 Cutter Plus</h1>

- 作者 Author: 莫yis
- 版本 Version: 2.10
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
            <li><a href="#General-Crafting-Tree">通用加工图 General Crafting Tree</a></li>
            <li>
            <a href="#Vanilla-Support">原版支持 Vanilla Support</a>
                <ol>
                    <li><a href="#Building-Blocks">建筑方块 Building Blocks</a></li>
                    <li><a href="#Decoration-Blocks">装饰性方块 Decoration Blocks</a></li>
                    <li><a href="#Redstone">红石 Redstone</a></li>
                    <li><a href="#Mod-Compatibility-minecraft">模组兼容 Mod Compatibility</a></li>
                </ol>
            </li>
            <li>
                <a href="#tconstruct">匠魂支持 Tinkers' Construct Support</a>
                <ol>
                    <li><a href="#Tinkers-General-Items">Tinkers' General Items</a></li>
                    <li><a href="#Tinkers-Smeltery">Tinkers' Smeltery</a></li>
                    <li><a href="#Mod-Compatibility-tconstruct">模组兼容 Mod Compatibility</a></li>
                </ol>
            </li>
            <li>
                <a href="#create">机械动力支持 Create Support</a>
                <ol>
                    <li><a href="#Create-Palettes">机械动力建筑方块 Create Palettes</a></li>
                    <li><a href="#Create-items">机械动力 Create</a></li>
                    <li><a href="#Mod-Compatibility-create">模组兼容 Mod Compatibility</a></li>
                </ol>
            </li>
            <li>
                <a href="#twilightforest">暮色森林支持 The Twilight Forest Support</a>
                <ol>
                    <li><a href="#Twilight-Forest">暮色森林 Twilight Forest</a></li>
                    <li><a href="#Mod-Compatibility-twilightforest">模组兼容 Mod Compatibility</a></li>
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

- 一个轻量级数据包，添加了大量切石机的工作配方。
- 你甚至可以用切石机切木头！ Emmm... 在生活中是可以的。
- 从版本 “2.4” 开始，使用 “Forge” 的通用矿物词典标签。
- 未加载的配方使用 “空气” 填充，保证多个模组之间兼容。
- “模组兼容” 是指从其他模组的物品加工到本模组时使用的配方。
- 在 “特性” 目录中，除 “模组兼容” 外，都代表了每个模组的物品栏的名称。
- 如果觉得空气配方碍眼，可以将没有的模组对应的以 “support” 开头的文件夹删除：
    - minecraft: 《Minecraft》是最早支持的内容。
    - tconstruct: 《匠魂 - 1.16.5》从版本 “2.4” 开始支持。
    - create: 《机械动力 - 1.16.5》从版本 “2.9” 开始支持。
    - twilightforest: 《暮色森林 - 1.16.5》从版本 “2.10” 开始支持。
- 符号说明：
    - <==>：代表两边都能加工。
    - -->>：代表只能向右边加工。
    - <<--：代表只能向左边加工。
    -   ◻ ：代表一个词。

<br>

- A lightweight data package that adds a large number of working formulas for stone-cutter.
- You can even cut wood with a stone-cutter! Emmm... It's OK in life.
- Starting with version "2.4", use the general mineral dictionary label of "Forge".
- Unloaded recipes are filled with "air" to ensure compatibility between multiple mods.
- "Mod Compatibility" refers to the recipes used when processing from the items of other mods to this mod.
- In the "Features" directory, except for "Mod Compatibility", it represents the name of the inventory of each mod.
- If you think the air recipe is eye-catching, you can delete the folder starting with "support" corresponding to the uninstalled mod:
    - minecraft: "Minecraft" was the first supported content.
    - tconstruct: "Tinkers' Construct - 1.16.5" is supported from version "2.4".
    - create: "Create - 1.16.5" is supported from version "2.9".
    - twilightforest： "The Twilight Forest - 1.16.5" is supported from version "2.10".
- Symbol description:
    - <==>: It means that both sides can be processed.
    - -->>: It means that it can only be processed to the right.
    - <<--: It means that it can only be processed to the left.
    -   ◻ : It means that a word.

<a href="#Contents">回到目录 Back to contents</a>
<h2 id="Features">特性 Features</h2>

- 要经过烧炼才能获得的方块无法从切石机获得，如平滑石头。
- 切石机只能加工固态物品和没有NBT标签的物品（从设计的角度上来看）。
- 同一类的方块（材质不同）之间可以相互转化（方块，楼梯，台阶，墙）。
- 苔石和苔石砖是由圆石和石砖加工而来，故不能相互转化。其他情况类似。
- 楼梯可以加工成对应的台阶。

<br>

- Blocks that can only be obtained by burning cannot be obtained from a stone cutter, such as the smooth_stones.
- The stone-cutter can only process solid articles and articles without NBT label.(From the design point of view.)
- Blocks of the same type (with different appearance) can be transformed into each other (block, stair, slab, wall).
- The mossy_cobblestone and the mossy_stone_bricks are processed from the cobblestone and the stone_bricks, so they can not be transformed into each other.Other situations are similar.
- Stairs can be processed into corresponding slab.

<a href="#Contents">回到目录 Back to contents</a>
<h3 id="General-Crafting-Tree">通用加工图 General Crafting Tree</h3>

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
------------------------------------------------------------------
木台阶 ------------>>  木棍 [1] <<---- 木楼梯
树叶 -------------->>  木棍 [1] <<---- 树苗
木栅栏 ------------>>  木棍 [2] <<---- 木压力板
木板 -------------->>  木棍 [2]
木门 -------------->>  木棍 [4] <<---- 木活板门
床 ---------------->>  木棍 [4]
船 ---------------->>  木棍 [6]
木头(菌核) --------->>  木棍 [8] <<---- 原木(菌柄)
去皮原木(去皮菌柄) -->>  木棍 [8] <<---- 去皮木头(去皮菌核)

wooden_slab ------------------>>  stick [1] <<-- wooden_stairs
leaves ----------------------->>  stick [1] <<-- sapling
wooden_fence ----------------->>  stick [2] <<-- wooden_pressure_plate
planks ----------------------->>  stick [2]
wooden_door ------------------>>  stick [4] <<-- wooden_trapdoor
beds ------------------------->>  stick [4]
boat ------------------------->>  stick [6]
wood(hyphae) ----------------->>  stick [8] <<-- log(stem)
stripped_log(stripped_stem) -->>  stick [8] <<-- stripped_wood(stripped_hyphae)
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="Vanilla-Support">原版支持 Vanilla Support</h3>
<h4 id="Building-Blocks">建筑方块 Building Blocks</h4>

```
------------------------------------------------------------------
(方块)
紫珀块 <=========>  紫珀柱
花岗岩 <=========>  磨制花岗岩
闪长岩 <=========>  磨制闪长岩
安山岩 <=========>  磨制安山岩
玄武岩 <=========>  磨制玄武岩
末地石 <=========>  末地石砖
下界砖块 <=======>  錾制下界砖块
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

书架 ----------->>  木棍 [6]
玻璃(染色) ------>>  玻璃板(染色) [3]
滴水石块 -------->>  滴水石锥
石头 ----------->>  石头按钮
黑石 ----------->>  磨制黑石按钮 <<-- 磨制黑石
紫水晶块 -------->>  紫水晶碎片
紫水晶簇 -------->>  紫水晶碎片 [3]
蓝冰 ----------->>  浮冰 ----->> 冰
石英块 ---------->>  下界石英
下界砖台阶 ------>>  下界砖 [2] <<-- 下界砖楼梯
下界砖块 -------->>  下界砖 [4]
砖台阶 ---------->>  红砖 [2] <<---- 砖楼梯
砖块 ----------->>  红砖 [4]
铁块 ----------->>  铁锭 [9] --->> 铁粒 [9]
金块 ----------->>  金锭 [9] -->> 金粒[9]
下界合金块 ------>>  下界合金锭 [9]
钻石块 ---------->>  钻石 [9]
绿宝石块 -------->>  绿宝石 [9]
青金石块 -------->>  青金石 [9]
海晶石砖台阶 ----->>  海晶石台阶
海晶石砖楼梯 ----->>  海晶石楼梯
海晶石砖 -------->>  海晶石 -->>  海晶石碎片 <<-- 海晶灯

（铜质方块）
(先) 打蜡的 -->>  未打蜡的
(后) 氧化的 -->>  锈蚀的 -->> 斑驳的 -->> 新的
块状的 <======>  切制的
楼梯 -->>  台阶 ------>> 铜锭 [4]
楼梯 -->>  铜锭 [4]
铜块 -->>  铜锭 [9] <<---- 切制铜块

------------------------------------------------------------------
(Block)
purpur_block <=====>  purpur_pillar
granite <==========>  polished_granite
diorite <==========>  polished_diorite
andesite <=========>  polished_andesite
basalt <===========>  polished_basalt
end_stone <========>  end_stone_bricks
nether_bricks <====>  chiseled_nether_bricks
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

bookshelf ------------->>  stick [6]
glass(stained) -------->>  glass_pane(stained) [3]
dripstone_block ------->>  pointed_dripstone
stone ----------------->>  stone_button
blackstone ------------>>  polished_blackstone_button
    <<------- polished_blackstone
amethyst_block -------->>  amethyst_shard
amethyst_cluster ------>>  amethyst_shard [3]
blue_ice -------------->>  packed_ice --->> ice
quartz_block ---------->>  quartz
nether_brick_slab ----->>  nether_brick [2] <<-- nether_brick_stairs
nether_bricks --------->>  nether_brick [4]
brick_slab ------------>>  brick [2] <--- brick_stairs
bricks ---------------->>  brick [4]
iron_block ------------>>  iron_ingot [9] -->>  iron_nugget [9]
gold_block ------------>>  gold_ingot [9] -->>  gold_nugget [9]
netherite_block ------->>  netherite_ingot [9]
diamond_block --------->>  diamond [9]
emerald_block --------->>  emerald [9]
lapis_block ----------->>  lapis_lazuli [9]
prismarine_brick_slab --->>  prismarine_slab
prismarine_brick_stairs ->>  prismarine_stairs
prismarine_bricks ---->>  prismarine --------->>
    prismarine_shard <<------- sea_lantern

(copper blocks)
(first) waxed ------>>  unwaxed
(second) oxidized -->>  weathered -->> exposed -->> new
block <=========>  cut
stairs ------------->>  slab ------>> copper_ingot [4]
stairs ------------->>  copper_ingot [4]
copper_block ------->>  copper_ingot [4] <<---- cut_copper
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Decoration-Blocks">装饰性方块 Decoration Blocks</h4>

```
------------------------------------------------------------------
黑石墙 <=====>  磨制黑石墙 <==>  磨制黑石砖墙

竹子 -------->>  木棍 [1] <<-- 脚手架
枯萎的灌木 --->>  木棍 [1]
梯子 -------->>  木棍 [2] <<-- 织布机
画 ---------->>  木棍 [2] <<-- 物品展示框
木告示牌 ----->>  木棍 [4] <<-- 制图台
制箭台 ------->>  木棍 [4] <<-- 锻造台
工作台 ------->>  木棍 [4] <<-- (灵魂)营火
堆肥桶 ------->>  木棍 [6] <<-- 盔甲架
木桶 --------->>  木棍 [6] <<-- 蜂箱
唱片机 ------->>  木棍 [8] <<-- 箱子

blackstone_wall <=====> polished_blackstone_wall
    <====> polished_blackstone_brick_wall

bamboo ----------->>  stick [1] <<-- scaffolding
dead_bush -------->>  stick [1]
ladder ----------->>  stick [2] <<-- loom
painting --------->>  stick [2] <<-- item_frame
wooden_sign ------>>  stick [4] <<-- cartography_table
fletching_table -->>  stick [4] <<-- smithing_table
crafting_table --->>  stick [4] <<-- (soul)campfire
composter -------->>  stick [6] <<-- armor_stand
barrel ----------->>  stick [6] <<-- beehive
jukebox ---------->>  stick [8] <<-- chest
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Redstone">红石 Redstone</h4>

```
------------------------------------------------------------------
木栅栏门 ----->> 木棍 [4] <<-- 讲台
陷阱箱 -------->> 木棍 [8] <<-- 音符盒

wooden_fence_gate -->> stick [4] <<-- lectern
trapped_chest ------>> stick [8] <<-- note_block
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility-minecraft">模组兼容 Mod Compatibility</h4>

```
------------------------------------------------------------------
(◻ = 花岗岩 / 闪长岩 / 安山岩)
(机械动力 ---->> (磨制)◻)
◻砖          方纹◻砖
竖纹◻         ◻铺路石
层叠◻         生苔◻
生草◻         ◻砖楼梯
方纹◻砖楼梯    ◻铺路石楼梯
◻砖台阶       方纹◻砖台阶
◻铺路石台阶    ◻砖墙
方纹◻砖墙      ◻铺路石墙

(机械动力 ------->> 木棍 [2])
大齿轮       水车
安山机壳     黄铜机壳
铜机壳       暗影机壳
光辉机壳

(匠魂 ------->> 木棍 [4])
wooden_sign      wooden_fence_gate

(暮色森林 ------->> 木棍 [4])
木告示牌        木栅栏门

(◻ = granite / diorite / andesite)
(Create -------->> (polished)◻)
◻_bricks                   fancy_◻_bricks
◻_pillar                   paved_◻
layered_◻                  mossy_◻
overgrown_◻                ◻_bricks_stairs
fancy_◻_bricks_stairs      paved_◻_stairs
◻_bricks_slab              fancy_◻_bricks_slab
paved_◻_slab               ◻_bricks_wall
fancy_◻_bricks_wall        paved_◻_wall

(Create ------>> stick [2])
large_cogwheel         water_wheel
andesite_casing        brass_casing
copper_casing          shadow_steel_casing
refined_radiance_casing

(Tinkers' Construct ------>> stick [4])
wooden_sign      wooden_fence_gate

(The Twilight Forest ------>> stick [4])
wooden_sign      wooden_fence_gate
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
seared_bricks_stairs <===> seared_stone_stairs
seared_bricks_slab <====> seared_stone_slab

seared_bricks_stairs ---->>  seared_brick_slab
seared_paver_stairs ----->>  seared_paver_slab
seared_cobble_stairs ---->>  seared_cobble_slab
seared_bricks ----------->>  seared_brick [4]
seared_bricks_stairs ---->>  seared_brick [2] <<-- seared_bricks_slab
seared_glass ------------>>  seared_glass_pane [3]

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
<h4 id="Mod-Compatibility-tconstruct">模组兼容 Mod Compatibility</h4>

```
------------------------------------------------------------------
(◻ = 铜)
(forge ----->> ◻)
◻锭    ◻粒    ◻矿石    ◻块

(原版)
下界合金锭 -->> netherite_nugget
黑曜石 -->> obsidian_pane

(◻ = copper)
(forge ----->> ◻)
◻_ingot    ◻_nugget    ◻_ore    ◻_block

(Vanilla)
netherite_ingot -->> netherite_nugget
obsidian -->> obsidian_pane
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="create">机械动力支持 Create Support</h3>
<h4 id="Create-Palettes">机械动力建筑方块 Create Palettes</h4>

```
------------------------------------------------------------------
(板)
十字玻璃窗 ----------->>  十字玻璃窗户板 [3]
边框玻璃 ------------->>  边框玻璃板 [3]
竖直边框玻璃(竖) ------>>  竖直边框玻璃板(竖) [3]
竖直边框玻璃(横) ------>>  竖直边框玻璃板(横) [3]
金合欢窗户 ----------->>  金合欢窗户板 [3]
白桦窗户 ------------->>  白桦窗户板 [3]
绯红窗户 ------------->>  绯红窗户板 [3]
深色橡木窗户 ---------->>  深色橡木窗户板 [3]
丛林窗户 ------------->>  丛林窗户板 [3]
橡木窗户 ------------->>  橡木窗户板 [3]
华丽铁窗户 ----------->>  华丽铁窗户板 [3]
云杉窗户 ------------->>  云杉窗户板 [3]
诡异木窗户 ----------->>  诡异木窗户板 [3]

(块 / 楼梯 / 台阶 / 墙)

(◻ = 花岗岩 / 闪长岩 / 安山岩)
◻砖 <======>  方纹◻砖 <=======>  竖纹◻
    <======>  ◻铺路石 <=======>  层叠◻
    <======>  生苔◻ <========>  生草◻
(◻ = 石灰岩 / 风化石灰岩 / 白云岩 / 辉长岩 / 熔渣 / 深色熔渣)
◻ <========>  磨制◻ <==========>  ◻砖
    <======>  方纹◻砖 <========>  竖纹◻
    <======>  ◻铺路石 <========>  层叠◻
    <======>  錾制◻ <==========>  生苔◻
    <======>  生草◻

(pane)
tiled_glass --------------->>  tiled_glass_pane [3]
framed_glass -------------->>  framed_glass_pane [3]
vertical_framed_glass ----->>  vertical_framed_glass_pane [3]
horizontal_framed_glass --->>  horizontal_framed_glass_pane [3]
acacia_window ------------->>  acacia_window_pane [3]
birch_window -------------->>  birch_window_pane [3]
crimson_window ------------>>  crimson_window_pane [3]
dark_oak_window ----------->>  dark_oak_window_pane [3]
jungle_window ------------->>  jungle_window_pane [3]
oak_window ---------------->>  oak_window_pane [3]
ornate_iron_window -------->>  ornate_iron_window_pane [3]
spruce_window ------------->>  spruce_window_pane [3]
warped_window ------------->>  warped_window_pane [3]

(block / stairs / slab / wall)

(◻ = granite / diorite / andesite)
◻_bricks <===>  fancy_◻_bricks <===>  ◻_pillar
    <========>  paved_◻ <==========>  layered_◻
    <========>  mossy_◻ <==========>  overgrown_◻
(◻ = limestone / weathered_limestone / dolomite / gabbro / scoria / dark_scoria)
 <=========>  polished_◻ <========>  ◻_bricks
    <======>  fancy_◻_bricks <====>  ◻_pillar
    <======>  paved_◻ <===========>  layered_◻
    <======>  chiseled_◻ <========>  mossy_◻
    <======>  overgrown_◻
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Create-items">机械动力 Create</h4>

```
------------------------------------------------------------------
(块 -->> 锭 [9] -->> 粒 [9])
铜     锌     黄铜

(block -->> ingot [9] -->> nugget [9])
copper         zinc        brass
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility-create">模组兼容 Mod Compatibility</h4>

```
------------------------------------------------------------------
(◻ = 铜)
(forge ----->> ◻)
◻锭    ◻粒    ◻矿石    ◻块

(◻ = (磨制)花岗岩 / (磨制)闪长岩 / (磨制)安山岩)
(原版)
◻砖楼梯
方纹◻砖楼梯    ◻铺路石楼梯
◻砖台阶       方纹◻砖台阶
◻铺路石台阶    ◻砖墙
方纹◻砖墙      ◻铺路石墙

(◻ = copper)
(forge ----->> ◻)
◻_ingot    ◻_nugget    ◻_ore    ◻_block

(◻ = (polished)granite / (polished)diorite / (polished)andesite)
(Vanilla)
◻_bricks_stairs
fancy_◻_bricks_stairs      paved_◻_stairs
◻_bricks_slab              fancy_◻_bricks_slab
paved_◻_slab               ◻_bricks_wall
fancy_◻_bricks_wall        paved_◻_wall
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="twilightforest">暮色森林支持 The Twilight Forest Support</h3>
<h4 id="Twilight-Forest">暮色森林 Twilight Forest</h4>

```
------------------------------------------------------------------
铁木块 ------->>  铁木锭
炽铁块 ------->>  炽铁锭
骑士金属块 ---->>  骑士金属锭

城堡砖 <================>  磨损城堡砖
黑纹城堡砖瓦 <===========>  黑纹城堡砖柱
粗纹城堡砖瓦 <===========>  粗纹城堡砖柱
娜迦石楼梯（左） <========>  娜迦石楼梯（右）
风化的娜迦石楼梯（左） <===>  风化的娜迦石楼梯（右）
娜迦苔石楼梯（左） <======>  娜迦苔石楼梯（右）
迷宫石头 <==> 迷宫石砖 <==>  装饰迷宫石砖
    <==> 錾制迷宫石头 <==>  迷宫石沿 <==> 迷宫镶石

ironwood_block ------->>  ironwood_ingot
fiery_block ---------->>  fiery_ingot
knightmetal_block ---->>  knightmetal_ingot

castle_brick <======================>  castle_brick_worn
castle_pillar_encased <=============>  castle_pillar_encased_tile
castle_pillar_bold <================>  castle_pillar_bold_tile
nagastone_stairs_left <=============>  nagastone_stairs_right
nagastone_stairs_weathered_left <===>  nagastone_stairs_right
nagastone_stairs_mossy_left <=======>  nagastone_stairs_mossy_right
maze_stone <==> maze_stone_brick <==>  maze_stone_decorative
    <==> maze_stone_chiseled <==> maze_stone_border <==> maze_stone_mosaic
------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility-twilightforest">模组兼容 Mod Compatibility</h4>

```
------------------------------------------------------------------

------------------------------------------------------------------
```
<a href="#Contents">回到目录 Back to contents</a>
<h2 id="Update">更新内容 Update</h2>

- 修改目录部分结构。
- 补充原版和机械动力兼容性内容。
- 完成对 暮色森林 的支持。
- 更新 README。

<h2 id="Update-Plan">计划更新 Update Plan</h2>

- 支持 暮色森林 The Twilight Forest
- 支持 超多生物群系 Biomes O' Plenty
- 支持 凿子 Chisel
- 支持 长沼蓝调 Bayou Blues
- 支持 秋原 Autumnity
- 支持 夸克 Quark
- 支持 Supplementaries
- 支持更多1.16.5的模组。

<a href="#Contents">回到目录 Back to contents</a>
<h2 id="Usage">使用方式 Usage</h2>

- Github: 右上角点击**绿色**的 "**Code**" 再点击 "**Download ZIP**"。
- Gitee: 右上角点击**橙色**的 "**克隆/下载**" 再点击 "**下载ZIP**"。

<br>

- 如果你打算将数据包放入存档中，请解压在 ".minecraft\\saves\\(存档名称)\\datapacks\\" 目录下。
- 如果你正准备新建世界，请将解压出的文件夹添加到游戏中。
- 如果你打算加载到已经启动的游戏或服务器中，请在后台或以3级操作员身份键入 "/reload" 以加载数据包。
- 相关疑问请查询 Minecraft Wiki。

<br>

- Github: Click the **green** "**Code**" in the upper right corner and then click "**Download ZIP**".
- If you plan to put the datapack into the archive, please unzip it in the ".minecraft\\saves\\(save name)\\datapacks\\" directory.
- If you are preparing to create a new world, please add the extracted folder to the game.
- If you plan to load into a game or server that has already started, please type "/reload" from the console or as a level 3 operator.
- For questions, please check the Minecraft Wiki.

<a href="#Contents">回到目录 Back to contents</a>
<h2 id="Warming">注意 Warming</h2>

- 与模组不同，数据包仅对单个世界有效。
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
