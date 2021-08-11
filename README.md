## 切石机增强 Cutter Plus
- 作者 Author: 莫yis
- 版本 Version: 0.2
- 支持版本 Supported version: 1.16.5
- Github: https://github.com/Mo-yis/Cutter_Plus
- Gitee: https://gitee.com/Mo-yis/Cutter_Plus

## 献辞 Dedication

    谨将此数据包, 献给所有努力生存的方块人!

    This datapack is dedicated to all those who strive to survive.

## 说明 Explain
- 一个简单的数据包, 仅使用一种合成方式, 方便合成.
- 你甚至可以用切石机切木头 ! Emmm... 生活中是可以.

## 特性 Features
- 在不破坏原版游戏平衡的情况下添加大量切石机的工作配方.
- 平滑石头等要经过烧炼才能得到的方块无法从切石机获得.

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

木台阶 wooden_slab                  木楼梯 wooden_stairs
树苗 sapling                        树叶 leaves
竹子 bamboo                         脚手架 scaffolding
枯萎的灌木 dead_bush

            分解成 2 个木棍 Break it down into two sticks

木栅栏 wooden_fence                 梯子 ladder
织布机 loom                         木板 planks

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

船 boat                              唱片机 jukebox
箱子 chest                           陷阱箱 trapped_chest
音符盒 note_block                    原木 log (菌柄 stem)
去皮原木 stripped_log (去皮菌柄 stripped_stem)
木头 wood (菌核 hyphae)
去皮木头 stripped_wood (去皮菌核 stripped_hyphae)

------------------------------------------------------------------
~~~~

### 石质物品加工图 Stony Crafting Tree
~~~~
------------------------------------------------------------------

- 相互转换

基岩 <==========> 命令方块
紫珀块 <========> 紫珀柱
花岗岩 <========> 磨制花岗岩
闪长岩 <========> 磨制闪长岩
安山岩 <========> 磨制安山岩
玄武岩 <========> 磨制玄武岩
末地石砖 <======> 末地石
下界砖块 <======> 錾制下界砖块

石头 <==========> 石砖 <=========> 錾制石砖
砂岩 <==========> 錾制砂岩 <=====> 切制砂岩
红砂岩 <========> 錾制红砂岩 <====> 切制红砂岩
黑石 <==========> 磨制黑石 <======> 磨制黑石砖 <====> 錾制磨制黑石砖
石英块 <========> 石英砖 <========> 錾制石英块 <====> 石英柱

- 单向转换

石头 ===========> 石头按钮
黑石 ===========> 磨制黑石按钮
磨制黑石 ========> 磨制黑石按钮
海晶石砖 ========> 海晶石
红色下界砖块 ====> 下界砖
下界砖块 ========> 下界砖
砖块 ============> 红砖

- Exchange
- Transform to
------------------------------------------------------------------
~~~~



 
<p>




## 使用方式 Usage
- Github: 右上角点击**绿色**的 "**Code**" 再点击 "**Download ZIP**" .
- Gitee: 右上角点击**橙色**的 "**克隆/下载**" 再点击 "**下载ZIP**" .

<p>

- 如果你打算将数据包放入存档中, 请解压在 ".minecraft\ saves\ (存档名称)\ datapacks\ " 目录下.
- 如果你正准备新建世界, 请解压下载的压缩包, 再从根目录重新压缩以添加到游戏中.
- 如果你打算加载到已经启动的服务器, 请在后台或以3级操作员身份键入 /reload 以加载数据包.

<p>

- Github: Click the **green** "**Code**" in the upper right corner and then click "**Download ZIP**".
- If you plan to put the datapack into the archive, please unzip it in the ".minecraft\ saves\ (archive name)\ datapacks\ " directory.
- If you are preparing to create a new world, please unzip the package and recompress it from the root directory to add it to the game.
- If you intend to load to a started server, type "/reload" from the console or as a level 3 operator.

## 注意 Warming
- 该数据包兼容新版本和旧版本.
- 请勿添加功能类似或相同的数据包.
- 合成配方可以通过json文件修改, 但不推荐这么做.

<p>

- This packet is compatible with new and old versions.
- Do not add datapack with similar or identical functions.
- Synthetic recipes can be modified through JSON files, but this is not recommended.
