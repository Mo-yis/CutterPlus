## 切石机增强 Cutter Plus
- 作者 Author: 莫yis
- 版本 Version: 1.1
- 支持版本 Supported version: 1.14.4 ~ 1.17.1
- Github: https://github.com/Mo-yis/Cutter_Plus
- Gitee: https://gitee.com/Mo-yis/Cutter_Plus

## 献辞 Dedication

    谨将此数据包, 献给所有努力生存的方块人!

    This datapack is dedicated to all those who strive to survive!

## 说明 Explain
- 一个轻量级数据包, 仅使用一种合成方式, 方便合成.
- 你甚至可以用切石机切木头 ! Emmm... 在生活中是可以.

<p>

- A simple packet, using only one synthesis method, is convenient for synthesis.
- You can even cut wood with a stone-cutter! Emmm... It's OK in life.

## 特性 Features
- 在不破坏原版游戏平衡的情况下添加大量切石机的工作配方.
- 要经过烧炼才能得到的方块无法从切石机获得, 比如平滑石头.
- 与其他物品一同合成出的同类方块间无法相互转换, 如苔石砖和苔石.

<p>

- Add a lot of working formula of stone-cutter without destroying the balance of the original game.
- Blocks that need to be burned cannot be obtained from stone-cutter, such as smooth stones.
- Similar blocks synthesized together with other items cannot be converted to each other, such as mossy_cobblestone and mossy_stone_bricks.

### 木制物品加工图 Wooden Crafting Tree
~~~~
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
        |-- 楼梯 stairs
        |-- 台阶 slab [2]
        |-- 按钮 button

------------------------------------------------------------------

        分解成 1 个木棍 Break it down into a sticks

木台阶 wooden_slab                    木楼梯 wooden_stairs
树苗 sapling                          树叶 leaves
竹子 bamboo                           脚手架 scaffolding
枯萎的灌木 dead_bush

        分解成 2 个木棍 Break it down into two sticks

木栅栏 wooden_fence                   梯子 ladder
织布机 loom                           木板 planks

        分解成 4 个木棍 Break it down into four sticks

木门 wooden_door                      木栅栏门 wooden_fence_gate
木告示牌 wooden_sign                  木压力板 wooden_pressure_plate
画 painting                           物品展示框 item_frame
讲台 lectern                          制图台 cartography_table
制箭台 fletching_table                锻造台 smithing_table
工作台 crafting_table

        分解成 6 个木棍 Break it down into six sticks

活板门 trapdoor                       堆肥桶 composter
营火 campfire                         灵魂营火 soul_campfire
盔甲架 armor_stand                    木桶 barrel
蜂箱 beehive                          书架 bookshelf

        分解成 8 个木棍 Break it down into eight sticks

船 boat                               唱片机 jukebox
箱子 chest                            陷阱箱 trapped_chest
音符盒 note_block                     原木 log (菌柄 stem)
去皮原木 stripped_log (去皮菌柄 stripped_stem)
木头 wood (菌核 hyphae)
去皮木头 stripped_wood (去皮菌核 stripped_hyphae)

------------------------------------------------------------------
~~~~

### 石质物品加工图 Stony Crafting Tree
~~~~
------------------------------------------------------------------

- 相互转换

(方块)

基岩 <===========>  命令方块

紫珀块 <=========>  紫珀柱
花岗岩 <=========>  磨制花岗岩
闪长岩 <=========>  磨制闪长岩
安山岩 <=========>  磨制安山岩
玄武岩 <=========>  磨制玄武岩
末地石 <=========>  末地石砖
下界砖块 <=======>  錾制下界砖块

石头 <===========>  石砖 <=========>  錾制石砖
砂岩 <===========>  錾制砂岩 <=====>  切制砂岩
红砂岩 <=========>  錾制红砂岩 <===>  切制红砂岩

黑石 <===========>  磨制黑石 <=====>  磨制黑石砖 <====> 錾制磨制黑石砖
石英块 <=========>  石英砖 <=======>  錾制石英块 <====> 石英柱

深板岩圆石 <======>  錾制深板岩 <===>  磨制深板岩
<================>
深板岩砖 <========>  深板岩瓦

(台阶)

花岗岩台阶 <======>  磨制花岗岩台阶
闪长岩台阶 <======>  磨制闪长岩台阶
安山岩台阶 <======>  磨制安山岩台阶
黑石台阶 <========>  磨制黑石台阶 <==>  磨制黑石砖台阶

- 单向转换

石头 ------------>>  石头按钮
黑石 ------------>>  磨制黑石按钮    <<------  磨制黑石
红色下界砖台阶 -->>  下界砖        <<--------  红色下界砖楼梯
红色下界砖块 ---->>  下界砖 [2]
下界砖台阶 ------>>  下界砖[2]       <<------  下界砖楼梯
下界砖块 -------->>  下界砖 [4]
砖台阶 ---------->>  红砖[2]       <<--------  砖楼梯
砖块 ------------>>  红砖 [4]

海晶石砖台阶 -> 海晶石台阶
海晶石砖 -------->>  海晶石 ---->>  海晶石碎片 <<------  海晶灯

- Exchange

(Block)

bedrock <==========>  command_block

purpur_block <=====>  purpur_pillar
granite <==========>  polished_granite
diorite <==========>  polished_diorite
andesite <=========>  polished_andesite
basalt <===========>  polished_basalt
end_stone <========>  end_stone_bricks
nether_bricks <====>  chiseled_nether_bricks

stone <============>  stone_bricks<=============>  chiseled_stone_bricks
sandstone <========>  chiseled_sandstone<=======>  cut_sandstone
red_sandstone <====>  chiseled_red_sandstone<===>  cut_red_sandstone

blackstone <=======>  polished_blackstone<======>
polished_blackstone_bricks <===========>  chiseled_polished_blackstone

quartz_block <=====>  quartz_bricks <============>
chiseled_quartz_block <================>  quartz_pillar

(Slab)

granite_slab <=====>  polished_granite_slab
diorite_slab <=====>  polished_diorite_slab
andesite_slab <====>  polished_andesite_slab
blackstone_slab <==>  polished_blackstone_slab <==> polished_blackstone_brick_slab


- Transform to

stone ----------------->>  stone_button
blackstone ------------>>  polished_blackstone_button <<- polished_blackstone
red_nether_brick_slab ->>  nether_brick          <<------ red_nether_brick_stairs
red_nether_bricks ----->>  nether_brick [2]
nether_brick_slab ----->>  nether_brick [2]     <<------- nether_brick_stairs
nether_bricks --------->>  nether_brick [4]
brick_slab ------------>>  brick [2]         <------------ brick_stairs
bricks ---------------->>  brick [4]

prismarine_brick_slab ->>  prismarine_slab
prismarine_bricks ----->>  prismarine --->>  prismarine_shard <<-- sea_lantern

------------------------------------------------------------------
~~~~

## 更新内容 Update
- 调整文件夹结构
- 对同类的石质台阶相互转换的支持.
- 添加部分物品的分解
- 更新数据包图标

## 计划更新 Update Plan
- 所有楼梯切割成台阶.
- 对同类的石质楼梯相互转换的支持.
- (1.17)铜可以除锈和脱蜡, 有蜡先脱蜡, 无蜡降低一级锈蚀程度.
- 对矿石块分解的支持, 如钻石块加工成9个钻石.

## 使用方式 Usage
- Github: 右上角点击**绿色**的 "**Code**" 再点击 "**Download ZIP**" .
- Gitee: 右上角点击**橙色**的 "**克隆/下载**" 再点击 "**下载ZIP**" .

<p>

- 如果你打算将数据包放入存档中, 请解压在 ".minecraft\ saves\ (存档名称)\ datapacks\ " 目录下.
- 如果你正准备新建世界, 请解压下载的压缩包, 再从根目录重新压缩以添加到游戏中.
- 如果你打算加载到已经启动的游戏或服务器, 请在后台或以3级操作员身份键入 /reload 以加载数据包.
- 详细步骤请查询 Minecraft Wiki.

<p>

- Github: Click the **green** "**Code**" in the upper right corner and then click "**Download ZIP**".
- If you plan to put the datapack into the archive, please unzip it in the ".minecraft\ saves\ (archive name)\ datapacks\ " directory.
- If you are preparing to create a new world, please unzip the package and recompress it from the root directory to add it to the game.
- If you plan to load into a game or server that has already started, please type "/reload" from the console or as a level 3 operator.
- For detailed steps, please query minecraft wiki.

## 注意 Warming
- 该数据包兼容旧版本, 但是不会专门针对旧版本进行维护.
- 请勿添加功能类似或相同的数据包.
- 合成配方可以通过JSON文件修改, 但不推荐这么做.
- 当数据包成功加载时, 游戏中会提示 "[< 数据包名称 >] Loading Successful !" .
- 版本低于1.15.2无法显示提示信息, 请以管理员身份键入命令"/datapack list"查看数据包信息.

<p>

- The datapack is compatible with the new version and the old version, but it will not be maintained specifically for the old version.
- Do not add datapack with similar or identical functions.
- Synthetic recipes can be modified through JSON files, but this is not recommended.
- When the datapack is successfully loaded, the game will prompt "[< datapack name >] Loading Successful !".
- The prompt message cannot be displayed in versions lower than 1.15.2. Please type the command "/datapack list" as an administrator to view the datapack information.
