<h1>切石机增强 Cutter Plus</h1>

- 版本 Version: 3.0.10
- 支持版本 Supported version: 1.14.4 ~ 1.18
- Github: https://github.com/Mo-yis/CutterPlus
- Gitee: https://gitee.com/Mo-yis/CutterPlus

<h2 id="Contents">目录 Contents</h2>
<ol>
    <li><a href="#Explain">说明 Explain</a></li>
    <li>
        <a href="#Features">特性 Features</a>
        <ol>
            <li><a href="#General-Crafting-Tree">通用加工图 General Crafting Tree</a></li>
            <li>
            <a href="#minecraft">原版支持 Vanilla Support</a>
                <ol>
                    <li><a href="#Building-Blocks-minecraft">建筑方块 Building Blocks</a></li>
                    <li><a href="#Decoration-Blocks-minecraft">装饰性方块 Decoration Blocks</a></li>
                    <li><a href="#Redstone-minecraft">红石 Redstone</a></li>
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
            <li>
                <a href="#biomesoplenty">超多生物群系支持 Biomes O' Plenty Support</a>
                <ol>
                    <li><a href="#Biomes-O-Plenty">Biomes O' Plenty</a></li>
                    <li><a href="#Mod-Compatibility-biomesoplenty">模组兼容 Mod Compatibility</a></li>
                </ol>
            </li>
            <li>
                <a href="#bayou_blues">长沼蓝调支持 Bayou Blues Support</a>
                <ol>
                    <li><a href="#Building-Blocks-bayou_blues">建筑方块 Building Blocks</a></li>
                    <li><a href="#Mod-Compatibility-bayou_blues">模组兼容 Mod Compatibility</a></li>
                </ol>
            </li>
            <li>
                <a href="#autumnity">秋原支持 Autumnity Support</a>
                <ol>
                    <li><a href="#Building-Blocks-autumnity">建筑方块 Building Blocks</a></li>
                    <li><a href="#Decoration-Blocks-autumnity">装饰性方块 Decoration Blocks</a></li>
                    <li><a href="#Mod-Compatibility-autumnity">模组兼容 Mod Compatibility</a></li>
                </ol>
            </li>
            <li>
                <a href="#quark">夸克支持 Quark Support</a>
                <ol>
                    <li><a href="#Building-Blocks-quark">建筑方块 Building Blocks</a></li>
                    <li><a href="#Decoration-Blocks-quark">装饰性方块 Decoration Blocks</a></li>
                    <li><a href="#Mod-Compatibility-quark">模组兼容 Mod Compatibility</a></li>
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
- 符号说明：
    - <==>：代表两边都能加工。
    - -->>：代表只能向右边加工。
    - <<--：代表只能向左边加工。
    - ◻ @ ：代表一个词。

<br>

- A lightweight data package that adds a large number of working formulas for stone-cutter.
- You can even cut wood with a stone-cutter! Emmm... It's OK in life.
- Starting with version "2.4", use the general mineral dictionary label of "Forge".
- Unloaded recipes are filled with "air" to ensure compatibility between multiple mods.
- "Mod Compatibility" refers to the recipes used when processing from the items of other mods to this mod.
- In the "Features" directory, except for "Mod Compatibility", it represents the name of the inventory of each mod.
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
- Symbol description:
    - <==>: It means that both sides can be processed.
    - -->>: It means that it can only be processed to the right.
    - <<--: It means that it can only be processed to the left.
    - ◻ @ : It means that a word.

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
原木 log (菌柄 stem)
    |-- 木板 planks [4]
        |-- 按钮 button
        |-- 台阶 slab [2]
        |-- 栅栏 fence
        |-- 楼梯 stairs
            |-- 台阶 slab
    |-- 木头 wood (菌核 hyphae)
        |-- 木板 planks [4]
            |-- 按钮 button
            |-- 台阶 slab [2]
            |-- 栅栏 fence
            |-- 楼梯 stairs
                |-- 台阶 slab
        |-- 去皮木头 stripped_wood (去皮菌核 stripped_hyphae)
            |-- 木板 planks [4]
                |-- 按钮 button
                |-- 台阶 slab [2]
                |-- 栅栏 fence
                |-- 楼梯 stairs
                    |-- 台阶 slab
    |-- 去皮原木 stripped_log (去皮菌柄 stripped_stem)
        |-- 木板 planks [4]
            |-- 按钮 button
            |-- 台阶 slab [2]
            |-- 栅栏 fence
            |-- 楼梯 stairs
                |-- 台阶 slab
        |-- 去皮木头 stripped_wood (去皮菌核 stripped_hyphae)
            |-- 木板 planks [4]
                |-- 按钮 button
                |-- 台阶 slab [2]
                |-- 栅栏 fence
                |-- 楼梯 stairs
                    |-- 台阶 slab

木台阶 ------------>>  木棍 [1] <<---- 木楼梯
树叶 -------------->>  木棍 [1] <<---- 树苗
木栅栏 ------------>>  木棍 [2] <<---- 木压力板
木板 -------------->>  木棍 [2]
木门 -------------->>  木棍 [4] <<---- 木活板门
床 ---------------->>  木棍 [4] <<---- 木栅栏门
木告示牌------------>>  木棍 [4]
船 ---------------->>  木棍 [6]
木头(菌核) --------->>  木棍 [8] <<---- 原木(菌柄)
去皮原木(去皮菌柄) -->>  木棍 [8] <<---- 去皮木头(去皮菌核)

------------------------------------------------------------------

wooden_slab ------------------>>  stick [1] <<-- wooden_stairs
leaves ----------------------->>  stick [1] <<-- sapling
wooden_fence ----------------->>  stick [2] <<-- wooden_pressure_plate
planks ----------------------->>  stick [2]
wooden_door ------------------>>  stick [4] <<-- wooden_trapdoor
beds ------------------------->>  stick [4]
boat ------------------------->>  stick [6]
wood(hyphae) ----------------->>  stick [8] <<-- log(stem)
stripped_log(stripped_stem) -->>  stick [8] <<-- stripped_wood(stripped_hyphae)
```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="minecraft">原版支持 Vanilla Support</h3>
<h4 id="Building-Blocks-minecraft">建筑方块 Building Blocks</h4>

```
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

(◻ = 台阶 / 楼梯)
石◻ <=========>  石砖◻
花岗岩◻ <======>  磨制花岗岩◻
闪长岩◻ <======>  磨制闪长岩◻
安山岩◻ <======>  磨制安山岩◻
黑石◻ <========>  磨制黑石◻ <===>  磨制黑石砖◻
深板岩圆石◻ <===>  磨制深板岩◻ <==> 深板岩砖◻ <==> 深板岩瓦◻

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
铁块 ----------->>  铁锭 [9]
金块 ----------->>  金锭 [9]
下界合金块 ------>>  下界合金锭 [9]
钻石块 ---------->>  钻石 [9]
绿宝石块 -------->>  绿宝石 [9]
青金石块 -------->>  青金石 [9]
海晶石砖台阶 ----->>  海晶石台阶
海晶石砖楼梯 ----->>  海晶石楼梯
海晶石砖 -------->>  海晶石 -->>  海晶石碎片 <<-- 海晶灯
石头 ------------>>  圆石
石台阶 ---------->>  圆石台阶
石楼梯 ---------->>  圆石楼梯
深板岩 ---------->>  深板岩圆石

（铜质方块）
(先) 打蜡的 -->>  未打蜡的
(后) 氧化的 -->>  锈蚀的 -->> 斑驳的 -->> 新的
切制铜台阶 --->>  铜锭 [1] <<-- 切制铜楼梯
铜块 -------->>  铜锭 [9]
切制铜块 ----->>  铜锭 [2]
------------------------------------------------------------------

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

(◻ = slab / stairs)
stone_◻ <=======>  stone_brick_◻
granite_◻ <=====>  polished_granite_◻
diorite_◻ <=====>  polished_diorite_◻
andesite_◻ <====>  polished_andesite_◻
blackstone_◻ <==>  polished_blackstone_◻ <==> polished_blackstone_brick_◻
cobbled_deepslate_◻ <=====> polished_deepslate_◻
    <===> deepslate_brick_◻ <===> deepslate_tile_◻

bookshelf ---------------->>  stick [6]
glass(stained) ----------->>  glass_pane(stained) [3]
dripstone_block ---------->>  pointed_dripstone
stone -------------------->>  stone_button
blackstone --------------->>  polished_blackstone_button <<-- polished_blackstone
amethyst_block ----------->>  amethyst_shard
amethyst_cluster --------->>  amethyst_shard [3]
blue_ice ----------------->>  packed_ice --->> ice
quartz_block ------------->>  quartz
nether_brick_slab -------->>  nether_brick [2] <<-- nether_brick_stairs
nether_bricks ------------>>  nether_brick [4]
brick_slab --------------->>  brick [2] <--- brick_stairs
bricks ------------------->>  brick [4]
iron_block --------------->>  iron_ingot [9]
gold_block --------------->>  gold_ingot [9]
netherite_block ---------->>  netherite_ingot [9]
diamond_block ------------>>  diamond [9]
emerald_block ------------>>  emerald [9]
lapis_block -------------->>  lapis_lazuli [9]
prismarine_brick_slab ---->>  prismarine_slab
prismarine_brick_stairs -->>  prismarine_stairs
prismarine_bricks -------->>  prismarine -->> prismarine_shard <<-- sea_lantern
stone -------------------->>  cobblestone
stone_slab --------------->>  cobblestone_slabe
stone_stairs ------------->>  cobblestone_stairs
deepslate ---------------->>  cobbled_deepslate

(copper blocks)
(first) waxed ------>>  unwaxed
(second) oxidized -->>  weathered -->> exposed -->> new
cut_slab ----------->>  copper_ingot [1] <<-- cut_stairs
copper_block ------->>  copper_ingot [9]
cut_copper --------->>  copper_ingot [2]
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Decoration-Blocks-minecraft">装饰性方块 Decoration Blocks</h4>

```
黑石墙 <=======> 磨制黑石墙 <==> 磨制黑石砖墙
深板岩圆石墙 <==> 深板岩瓦墙 <==> 深板岩砖墙 <==> 磨制深板岩墙

竹子 -------->>  木棍 [1] <<-- 脚手架
枯萎的灌木 --->>  木棍 [1]
梯子 -------->>  木棍 [2] <<-- 织布机
制图台 ------->>  木棍 [4]
制箭台 ------->>  木棍 [4] <<-- 锻造台
工作台 ------->>  木棍 [4] <<-- (灵魂)营火
堆肥桶 ------->>  木棍 [6] <<-- 盔甲架
木桶 --------->>  木棍 [6] <<-- 蜂箱
唱片机 ------->>  木棍 [8] <<-- 箱子

------------------------------------------------------------------

blackstone_wall <==> polished_blackstone_wall
    <=======> polished_blackstone_brick_wall
cobbled_deepslate_wall <==> deepslate_tile_wall
    <=======> deepslate_brick_wall <==> polished_deepslate_wall

bamboo ----------->>  stick [1] <<-- scaffolding
dead_bush -------->>  stick [1]
ladder ----------->>  stick [2] <<-- loom
wooden_sign ------>>  stick [4] <<-- cartography_table
fletching_table -->>  stick [4] <<-- smithing_table
crafting_table --->>  stick [4] <<-- (soul)campfire
composter -------->>  stick [6] <<-- armor_stand
barrel ----------->>  stick [6] <<-- beehive
jukebox ---------->>  stick [8] <<-- chest
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Redstone-minecraft">红石 Redstone</h4>

```
讲台 ------->> 木棍 [4]
陷阱箱 ------>> 木棍 [8] <<-- 音符盒

------------------------------------------------------------------

lectern ----------->> stick [4]
trapped_chest ----->> stick [8] <<-- note_block
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility-minecraft">模组兼容 Mod Compatibility</h4>

```
(◻ = 花岗岩 / 闪长岩 / 安山岩) (机械动力 -->> (磨制)◻)
◻砖           方纹◻砖
竖纹◻          ◻铺路石
层叠◻          生苔◻
生草◻          ◻砖楼梯
方纹◻砖楼梯     ◻铺路石楼梯
◻砖台阶        方纹◻砖台阶
◻铺路石台阶     ◻砖墙
方纹◻砖墙       ◻铺路石墙

(机械动力 ------->> 木棍 [2])
大齿轮       水车
安山机壳     黄铜机壳
铜机壳       暗影机壳
光辉机壳

(超多生物群系) 肉块 ------->>  腐肉
(超多生物群系) 芦苇 ------->>  木棍 [1] <<-- 红树根
(超多生物群系) 垂死木树枝 -->>  木棍 [1] <<-- 荆棘
(暮色森林) 巨型树叶 ------->>  木棍 [64]
(暮色森林) 巨型原木 ------->>  橡木木板 [64]
(暮色森林) 巨型圆石 ------->>  圆石 [64]
(暮色森林) 巨型黑曜石 ------>>  黑曜石 [64]
(长沼蓝调) 丝柏膝根 ------->>  木棍 [1] <<-- 大型丝柏膝根
(长沼蓝调) 丝柏树枝 ------->>  木棍 [1]
(长沼蓝调) 丝柏木告示牌 ---->>  木棍 [4] <<-- 丝柏木栅栏门
(秋原) 枫木告示牌 --------->>  木棍 [4] <<-- 枫木栅栏门
(夸克) 木柱 -------------->>  木棍 [1] <<-- 染色木台阶
(夸克) 染色木楼梯 --------->>  木棍 [1] <<-- (染色)竖直木台阶
(夸克) 书架 -------------->>  木棍 [6]
(夸克) 饲料槽 ------------>>  木棍 [2] <<-- 木梯子
(夸克) 木(陷阱)箱 --------->>  木棍 [8]
(夸克) 树篱 -------------->>  木棍 [1]

(夸克) 陶瓦片(彩色) <====> 陶瓦(彩色)
(夸克) 竖直木板 <========> 木板
(夸克) 岩浆砖 <==========> 岩浆块
(夸克) 竖直木台阶 <======> 木台阶
(夸克) 磨制花岗岩砖墙 <===> 花岗岩墙
(夸克) 磨制闪长岩砖墙 <===> 闪长岩墙
(夸克) 磨制安山岩砖墙 <===> 安山岩墙

------------------------------------------------------------------

(◻ = granite / diorite / andesite) (Create -->> (polished)◻)
◻_bricks                   fancy_◻_bricks
◻_pillar                   paved_◻
layered_◻                  mossy_◻
overgrown_◻                ◻_bricks_stairs
fancy_◻_bricks_stairs      paved_◻_stairs
◻_bricks_slab              fancy_◻_bricks_slab
paved_◻_slab               ◻_bricks_wall
fancy_◻_bricks_wall        paved_◻_wall

(Create ------>> stick [2])
large_cogwheel           water_wheel
andesite_casing          brass_casing
copper_casing            shadow_steel_casing
refined_radiance_casing

(Biomes O' Plenty) flesh -------->>  rotten_flesh
(Biomes O' Plenty) reed --------->>  stick [1] <<-- mangrove_root
(Biomes O' Plenty) dead_branch -->>  stick [1] <<-- bramble
(The Twilight Forest) giant_leaves ------->>  stick [64]
(The Twilight Forest) giant_log ---------->>  oak_planks [64]
(The Twilight Forest) giant_cobblestone -->>  cobblestone [64]
(The Twilight Forest) giant_obsidian ----->>  obsidian [64]
(Bayou Blues) cypress_knee -------->>  stick [1] <<-- large_cypress_knee
(Bayou Blues) cypress_branch ------>>  stick [1]
(Bayou Blues) cypress_fence_gate -->>  stick [4] <<-- large_sign
(Autumnity) maple_fence_gate ------>>  stick [4] <<-- maple_sign
(Quark) wooden_post ---->>  stick [1] <<-- stained_planks_slab
(Quark) stained_planks_stairs ----->>  stick [1] <<-- (stained_planks)_vertical_slab
(Quark) bookshelf ----------------->>  stick [6]
(Quark) feeding_trough ------------>>  stick [2] <<-- wooden_ladder
(Quark) wooden_(trapped_)chest ---->>  stick [8]
(Quark) hedge --------------------->>  stick [1]

(Quark) shingles(colored) <=====> terracotta(colored)
(Quark) vertical_planks <=======> planks
(Quark) magma_bricks <==========> magma_block
(Quark) wooden_vertical_slab <==> wooden_slab
(Quark) granite_bricks_wall <===> granite_wall
(Quark) diorite_bricks_wall <===> diorite_wall
(Quark) andesite_bricks_wall <==> andesite_wall
```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="tconstruct">匠魂支持 Tinkers' Construct Support</h3>
<h4 id="Tinkers-General-Items">Tinkers' General Items</h4>

```
mud_bricks ---->>  mud_bricks_stairs
mud_bricks ---->>  mud_bricks_slab [2]
lavawood ------>>  lavawood_stairs
lavawood ------>>  lava_slab [2]
blazewood ----->>  blazewood_stairs
blazewood ----->>  blazewood_slab [2]
nahuatl ------->>  nahuatl_stairs
nahuatl ------->>  nahuatl_slab [2]
nahuatl ------->>  nahuatl_fence

clear_glass ---------->>  clear_glass_pane [3]
soul_glass ----------->>  soul_glass_pane [3]
clear_stained_glass -->>  clear_stained_glass_pane [3]

(block -->> ingot [9])
copper              cobalt
slimesteet          tinkers_bronze
rose_gold           pig_iron
queens_slime        manyullyn
hepatizon
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Tinkers-Smeltery">Tinkers' Smeltery</h4>

```
seared_stone <=============>  seared_bricks <=======> 
    seared_fancy_bricks <==>  seared_triangle_bricks
seared_bricks_stairs <=====>  seared_stone_stairs
seared_bricks_slab <=======>  seared_stone_slab

seared_bricks ----------->>  seared_brick [4]
seared_bricks_stairs ---->>  seared_brick [2] <<-- seared_bricks_slab
seared_glass ------------>>  seared_glass_pane [3]
seared_stone ------------>>  seared_cobble
seared_paver_slab ------->>  seared_bricks_slab
seared_paver_stairs ----->>  seared_bricks_stairs
seared_triangle_bricks <<---- seared_paver -->> seared_bricks
seared_stone <<-------------- seared_paver -->> seared_fancy_bricks

scorched_bricks <=====>  chiseled_scorched_bricks <====>
    scorched_stone <==>  polished_scorched_stone

scorched_road_slab ------>>  scorched_bricks_slab
scorched_road_stairs ---->>  scorched_bricks_stairs
scorched_road ----------->>  scorched_stone
scorched_bricks --------->>  scorched_brick [4]
scorched_bricks_stairs -->>  scorched_brick [2] <<-- scorched_bricks_slab
scorched_glass ---------->>  scorched_glass_pane [3]
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility-tconstruct">模组兼容 Mod Compatibility</h4>

```
(◻ = 铜) (forge ----->> ◻)
◻锭    ◻矿石    ◻块

(原版) 黑曜石 -------->>  obsidian_pane
(超多生物群系) 泥巴 <===>  mud_bricks

------------------------------------------------------------------

(◻ = copper) (forge ----->> ◻)
◻_ingot    ◻_ore    ◻_block

(Vanilla) obsidian --------->>  obsidian_pane
(Biomes O' Plenty) mud <=====>  mud_bricks
```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="create">机械动力支持 Create Support</h3>
<h4 id="Create-Palettes">机械动力建筑方块 Create Palettes</h4>

```
玻璃 ------->>  玻璃板 [3]
窗户 ------->>  窗户板 [3]

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

------------------------------------------------------------------

glass ----------->>  glass_pane [3]
window ---------->>  window_pane [3]

(block / stairs / slab / wall)
    (◻ = granite / diorite / andesite)
    ◻_bricks <===>  fancy_◻_bricks <===>  ◻_pillar
        <========>  paved_◻ <==========>  layered_◻
        <========>  mossy_◻ <==========>  overgrown_◻
    (◻ = limestone / weathered_limestone / dolomite / gabbro / scoria / dark_scoria)
    ◻ <========>  polished_◻ <========>  ◻_bricks
        <======>  fancy_◻_bricks <====>  ◻_pillar
        <======>  paved_◻ <===========>  layered_◻
        <======>  chiseled_◻ <========>  mossy_◻
        <======>  overgrown_◻
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Create-items">机械动力 Create</h4>

```
(块 -->> 锭 [9])
铜     锌     黄铜

------------------------------------------------------------------

(block -->> ingot [9])
copper         zinc        brass
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility-create">模组兼容 Mod Compatibility</h4>

```
(◻ = 铜 / 锌) (forge ----->> ◻)
◻锭    ◻矿石    ◻块

(原版) (◻ = (磨制)花岗岩 / (磨制)闪长岩 / (磨制)安山岩)
◻砖楼梯
方纹◻砖楼梯      ◻铺路石楼梯
◻砖台阶         方纹◻砖台阶
◻铺路石台阶      ◻砖墙
方纹◻砖墙        ◻铺路石墙

(原版) (◻ = 花岗岩 / 闪长岩 / 安山岩)
◻台阶 ------>>  ◻圆石台阶
◻楼梯 ------>>  ◻圆石楼梯
◻墙 -------->>  ◻圆石墙

------------------------------------------------------------------

(◻ = copper / zinc) (forge ----->> ◻)
◻_ingot    ◻_ore    ◻_block

(Vanilla) (◻ = (polished)granite / (polished)diorite / (polished)andesite)
◻_bricks_stairs
fancy_◻_bricks_stairs      paved_◻_stairs
◻_bricks_slab              fancy_◻_bricks_slab
paved_◻_slab               ◻_bricks_wall
fancy_◻_bricks_wall        paved_◻_wall

(Vanilla) (◻ = granite / diorite / andesite)
◻_slab -------->>  ◻_cobblestone_slab
◻_stairs ------>>  ◻_cobblestone_stairs
◻_wall -------->>  ◻_cobblestone_wall
```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="twilightforest">暮色森林支持 The Twilight Forest Support</h3>
<h4 id="Twilight-Forest">暮色森林 Twilight Forest</h4>

```
铁木块 ------->>  铁木锭
炽铁块 ------->>  炽铁锭
骑士金属块 ---->>  骑士金属锭

磨损城堡砖楼梯 <=========>  城堡砖楼梯
城堡砖 <================>  磨损城堡砖
黑纹城堡砖瓦 <===========>  黑纹城堡砖柱
粗纹城堡砖瓦 <===========>  粗纹城堡砖柱
娜迦石楼梯（左） <========>  娜迦石楼梯（右）
风化的娜迦石楼梯（左） <===>  风化的娜迦石楼梯（右）
娜迦苔石楼梯（左） <======>  娜迦苔石楼梯（右）
迷宫石头 <==> 迷宫石砖 <==>  装饰迷宫石砖 <=======>
    錾制迷宫石头 <=======>  迷宫石沿 <==> 迷宫镶石

------------------------------------------------------------------

ironwood_block ------->>  ironwood_ingot
fiery_block ---------->>  fiery_ingot
knightmetal_block ---->>  knightmetal_ingot

castle_stairs_worn <================>  castle_stairs_brick
castle_brick <======================>  castle_brick_worn
castle_pillar_encased <=============>  castle_pillar_encased_tile
castle_pillar_bold <================>  castle_pillar_bold_tile
nagastone_stairs_left <=============>  nagastone_stairs_right
nagastone_stairs_weathered_left <===>  nagastone_stairs_right
nagastone_stairs_mossy_left <=======>  nagastone_stairs_mossy_right
maze_stone <==> maze_stone_brick <==>  maze_stone_decorative
    <==> maze_stone_chiseled <==> maze_stone_border <==> maze_stone_mosaic
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility-twilightforest">模组兼容 Mod Compatibility</h4>

```

```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="biomesoplenty">超多生物群系支持 Biomes O' Plenty Support</h3>
<h4 id="Biomes-O-Plenty">Biomes O' Plenty</h4>

```
白砂岩 <=======>  切制白砂岩 <=======> 錾制白砂岩
橙色砂岩 <=====>  切割的橙色砂岩 <====> 凿过的橙色砂岩
黑砂岩 <=======>  切割的黑色砂岩 <====> 凿过的黑色砂岩
白砂岩台阶 <====>  切制白砂岩台阶
橙色砂岩台阶 <==>  切割的橙色砂岩台阶
黑砂岩台阶 <====>  切割的黑色砂岩台阶

泥砖楼梯 <<------  泥砖 --------->> 泥砖台阶
泥砖楼梯 ------>>  泥砖(砖) [2] <<---- 泥砖台阶
泥砖 --------->>  泥砖(砖) [4]
下界水晶块 ---->>  下界水晶

------------------------------------------------------------------

white_sandstone <====> cut_white_sandstone <====> chiseled_white_sandstone
orange_sandstone <===> cut_orange_sandstone <===> chiseled_orange_sandstone
black_sandstone <====> cut_black_sandstone <====> chiseled_black_sandstone
white_sandstone_slab <====> cut_white_sandstone_slab
orange_sandstone_slab <===> cut_orange_sandstone_slab
black_sandstone_slab <====> cut_black_sandstone_slab

mud_brick_stairs <<------  mud_bricks ---->> mud_brick_slab
mud_brick_stairs ------>>  mud_brick [2] <<---- mud_brick_slab
mud_bricks ------------>>  mud_brick [4]
nether_crystal_block -->>  nether_crystal
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility-biomesoplenty">模组兼容 Mod Compatibility</h4>

```
(匠魂) mud_bricks <==> 泥巴

------------------------------------------------------------------

(Tinkers' Construct) mud_bricks <==> mud
```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="bayou_blues">长沼蓝调支持 Bayou Blues Support</h3>
<h4 id="Building-Blocks-bayou_blues">建筑方块 Building Blocks</h4>

```
水藻团台阶 [2] <<-- 水藻团 -->> 水藻团楼梯
须松罗块 -->>  须松罗
丝柏木 ---->>  丝柏树枝

------------------------------------------------------------------

algae_thatch_slab [2] <<-- algae_thatch -->> algae_thatch_stairs
beard_moss_block -->>  beard_moss
cypress_wood ------>>  cypress_branch
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility-bayou_blues">模组兼容 Mod Compatibility</h4>

```

```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="autumnity">秋原支持 Autumnity Support</h3>
<h4 id="Building-Blocks-autumnity">建筑方块 Building Blocks</h4>

```
蜗牛壳砖块 <====>  錾制蜗牛壳砖 <==> 蜗牛壳瓦块
蜗牛壳砖楼梯 <==>  蜗牛壳瓦楼梯
蜗牛壳砖台阶 <==>  蜗牛壳瓦台阶

溢满树液的枫木原木 -->> 枫木木板 [4] <<-- 溢满树液的枫木
蜗牛壳方块 -------->> 蜗牛壳碎片 [9]

------------------------------------------------------------------

snail_shell_bricks <========>  chiseled_snail_shell_bricks <==> snail_shell_tiles
snail_shell_brick_stairs <==>  snail_shell_tile_stairs
snail_shell_brick_slab <====>  snail_shell_tile_slab

sappy_maple_log ---->> maple_planks [4] <<-- sappy_maple_wood
snail_shell_block -->> snail_shell_piece [9]
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Decoration-Blocks-autumnity">装饰性方块 Building Blocks</h4>

```
蜗牛壳砖墙 <==> 蜗牛壳瓦墙

------------------------------------------------------------------

snail_shell_brick_wall <==> snail_shell_tile_wall
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility-autumnity">模组兼容 Mod Compatibility</h4>

```

```
<a href="#Contents">回到目录 Back to contents</a>
<h3 id="quark">夸克支持 Quark Support</h3>
<h4 id="Building-Blocks-quark">建筑方块 Building Blocks</h4>

```
楼梯 ------------>>  竖直台阶
镶框玻璃(染色) ---->>  镶框玻璃板(染色) [3]
染色台阶 [2] <<-----  染色木板 -->> 竖直染色台阶 [2]
黑云母块 --------->>  末影黑云母
锈化铁板块 ------->>  铁板块

(◻ = 草块 / 茅草 / 泥土砖 / 黯缚块 / 沙砖 / 雪砖 / 仙人掌绿块)
◻台阶 [2] <<-- ◻  -->> 竖直◻台阶 [2]
◻  -------->> ◻楼梯

台阶 <=======>  竖直台阶
染色木板 <====>  竖直染色木板
硫磺石 <======>  硫磺石砖
深板岩圆石 <==>  錾制深板岩 <==> 磨制深板岩 <==> 深板岩砖 <==> 深板岩瓦
黑云母块 <====>  錾制黑云母块 <==> 黑云母支柱 <==> 黑云母砖
冻土 <=======>  冻土砖
灵魂砂岩 <====>  灵魂砂岩砖 <==> 錾制灵魂砂岩 <==> 切制灵魂砂岩
仙人掌绿块 <==>  仙人掌绿支柱

(◻ = 大理石 / 石灰石 / 碧玉石 / 板岩 / 虚空石 / 幻境石)
◻ <====>  磨制◻ <=======> 磨制◻砖
    <==>  錾制磨制◻砖 <==> 磨制◻铺路石 <==> 磨制◻柱

(◻ = 台阶 / 楼梯 / 竖直台阶)
远古海晶石砖◻ <====>  远古海晶石◻
硫磺石◻ <=========>  硫磺石砖◻
深板岩圆石◻ <======>  磨制深板岩◻ <==> 深板岩砖◻ <==> 深板岩瓦◻
    (@ = 大理石 / 石灰石 / 碧玉石 / 板岩 / 虚空石 / 幻境石)
    @◻ <=====>  磨制@◻ <==> 磨制@砖◻
冻土◻ <=======>  冻土砖◻
灵魂砂岩◻ <====>  灵魂砂岩砖◻ <==> 切制灵魂砂岩◻
锈化铁板块◻ -->>  铁板块◻

------------------------------------------------------------------

stairs ---->> vertical_slabs
framed_glass(stained) ---->> framed_glass_pane(stained) [3]
stained_slab [2] <<-- stained_planks -->> stained_vertical_slab [2]
biotite_block -->> biotite
rusty_iron_plate -->> iron_plate

(◻ = turf / thatch / dirt_bricks / duskbound_block / sandy_bricks / snow_bricks / midori_block)
◻_slab [2] <<-- ◻  -->> ◻_vertical_slab [2]
◻  -->> ◻_stairs

slab <====> vertical_slab
stained_planks <====> vertical_stained_planks
brimstone <==> brimstone_bricks
cobbled_deepslate <==> chiseled_deepslate <======>
    polished_deepslate <==> deepslate_bricks <==> deepslate_tiles
biotite_block <==> chiseled_biotite_block <==> biotite_pillar <==> biotite_bricks
permafrost <==> permafrost_bricks
soul_sandstone <==> soul_sandstone_bricks <==> chiseled_soul_sandstone <==> cut_soul_sandstone
midori_block <==> midori_pillar

(◻ = marble / limestone / jasper / slate / basalt / myalite)
◻ <====> polished_◻ <=========> ◻_bricks
    <==> chiseled_◻_bricks <==> ◻_pavement <==> ◻_pillar

(◻ = slab / stairs / vertical_slab)
elder_prismarine_bricks_◻ <====> elder_prismarine_◻
brimstone_◻ <==> brimstone_bricks_◻
cobbled_deepslate_◻ <==> polished_deepslate_◻ <==> deepslate_brick_◻ <==> deepslate_tile_◻
    (@ = marble / limestone / jasper / slate / basalt / myalite)
    @_◻ <==> polished_@_◻ <==> @_bricks_◻
permafrost_◻ <==> permafrost_bricks_◻
soul_sandstone_◻ <==> soul_sandstone_bricks_◻ <==> cut_soul_sandstone_◻
rusty_iron_plate_◻ -->> iron_plate_◻
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Decoration-Blocks-quark">装饰性方块 Building Blocks</h4>

```
刚玉(彩色) ---->> 刚玉板(彩色) [2]
深板岩圆石墙 <==> 深板岩瓦墙 <==> 深板岩砖墙 <==> 磨制深板岩墙

(◻ = 大理石 / 石灰石 / 碧玉石 / 板岩 / 虚空石 / 幻境石 / 冻土)
◻墙 <==> 磨制◻砖墙

------------------------------------------------------------------

crystal(colored) ---->> crystal_pane(colored) [2]
cobbled_deepslate_wall <==> deepslate_tile_wall
    <=======> deepslate_brick_wall <==> polished_deepslate_wall

(◻ = marble / limestone / jasper / slate / basalt / myalite / permafrost)
◻_wall <==> ◻_bricks_wall
```
<a href="#Contents">回到目录 Back to contents</a>
<h4 id="Mod-Compatibility-quark">模组兼容 Mod Compatibility</h4>

```
(原版) 木(菌核) ---->>  木柱 [3]
(原版) 木板 <========>  竖直木板
(原版) 岩浆块 <======>  岩浆砖
(原版) 木台阶 <======>  竖直木台阶
(原版) 花岗岩墙 <====>  磨制花岗岩砖墙
(原版) 闪长岩墙 <====>  磨制闪长岩砖墙
(原版) 安山岩墙 <====>  磨制安山岩砖墙

------------------------------------------------------------------

(Vanilla) wood(hyphae) ---->> wood_post [3]
(Vanilla) planks <==> vertical_planks
(Vanilla) magma_block <==> magma_bricks
(Vanilla) wooden_slab <==> wooden_vertical_slab
(Vanilla) granite_wall <==> granite_bricks_wall
(Vanilla) diorite_wall <==> diorite_bricks_wall
(Vanilla) andesite_wall <==> andesite_bricks_wall
```
<a href="#Contents">回到目录 Back to contents</a>
<h2 id="Update">更新内容 Update</h2>

- 调整 support-bayou_blues 文件夹结构，增加 tree 文件
- 添加 bayou_blues: cypress_wood -->>  cypress_branch
- 更新 README

<h2 id="Update-Plan">计划更新 Update Plan</h2>

- 更新模组内容支持
- 添加更多模组间兼容性配方
- 调整文件夹目录、规范文件命名
- 支持更多1.16.5的模组

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
- Extremely sorry for my bad English.

<a href="#Contents">回到目录 Back to contents</a>
