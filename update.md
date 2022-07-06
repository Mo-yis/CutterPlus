### [2022-06-06 : v4.0.1]
- 修改单词通配符为 □
- 更新 README

### [2022-06-06 : v4.0.0]
- 调整 support-quark 和 support-minecraft 的文件夹结构与文件命名
- 调整 support-quark 的部分配方:
    - > * [+] (minecraft) polished_□_stairs -> □_bricks_stairs
      > * [+] (minecraft) □_stairs -> □_bricks_stairs
      >> □ = granite | diorite | andesite
    - > * [+] (minecraft) polished_□_slab -> □_bricks_slab
      > * [+] (minecraft) □_slab -> □_bricks_slab
      >> □ = granite | diorite | andesite
    - [+] dirty_glass -> dirty_glass_pane
- 调整 support-minecraft 的部分配方:
    - > * [+] (quark) □_bricks_stairs -> polished_□_stairs
      > * [+] (quark) □_bricks_stairs -> □_stairs
      >> □ = granite | diorite | andesite
    - > * [+] (quark) □_bricks_slab -> polished_□_slab
      > * [+] (quark) □_bricks_slab -> □_slab
      >> □ = granite | diorite | andesite
- 为 support-quark 添加 tree 文件
- 更新 support-minecraft 的 tree 文件
- 提升数据包等级至 9
- 更改数据包下载方式

### [2022-06-05 : v3.1.2]
- 调整 support-quark 文件夹结构
- 添加 support-quark tag:
    - stony_block/quark_andesite
    - stony_block/quark_diorite
    - stony_block/quark_granite
- 调整 support-quark 的部分配方:
    - [+] (minecraft) tag:logs&stems -> vertical_planks [4]
    - > [+] □_bricks <=> chiseled_□_bricks <=> □_pavement <=> □_pillar
      >> □ = granite | diorite | andesite
    - > * [+] (minecraft) polished_□ -> chiseled_□_bricks
      > * [+] (minecraft) polished_□ -> □_pavement
      > * [+] (minecraft) polished_□ -> □_pillar
      >> □ = granite | diorite | andesite
- 调整 support-minecraft 的部分配方:
    - [+] (quark) sturdy_stone -> cobblestone
    - > * [+] (quark) tag:stony_block/quark_□ -> □
      > * [+] (quark) tag:stony_block/quark_□ -> polished_□
      >> □ = granite | diorite | andesite

### [2022-06-05 : v3.1.1]
- 调整 support-quark 的部分配方:
    - [+] granite_bricks_stairs -> granite_bricks_slab <- granite_bricks_vertical_slab
    - [+] diorite_bricks_stairs -> diorite_bricks_slab <- diorite_bricks_vertical_slab
    - [+] andesite_bricks_stairs -> andesite_bricks_slab <- andesite_bricks_vertical_slab

### [2022-06-04 : v3.1.0]
- 调整 support-quark 文件夹结构
- 调整 support-quark 的部分配方:
    - [+] dirt_bricks -> dirt_bricks_wall
    - [+] vanilla_basalt_bricks_stairs -> vanilla_basalt_bricks_vertical_slab <- vanilla_basalt_bricks_slab
    - [+] iron_plate -> iron_plate_slab [2]
    - [+] iron_plate -> iron_plate_vertical_slab [2]
    - [+] rusty_iron_plate -> rusty_iron_plate_slab [2]
    - [+] rusty_iron_plate -> rusty_iron_plate_vertical_slab [2]
    - [-] iron_plate_stairs -> rusty_iron_plate_stairs
    - [+] sandy_bricks -> sandy_bricks_wall
    - [+] snow_bricks -> snow_bricks_wall
    - [+] brimstone_wall <=> brimstone_bricks_wall
- 更新 README

### [2022-06-03 : v3.0.15]
- 修复语言切换链接

### [2022-06-03 : v3.0.14]
- 将英文从 README 中分离
- 新增繁體中文

### [2022-06-03 : v3.0.13]
- 特性目录中的配方全部迁移到 CutterPlus WIKI: https://github.com/Mo-yis/CutterPlus/wiki
- 更新 README

### [2022-06-02 : v3.0.12]
- 更换开源协议. 现在的协议为 DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
- 移除 Gitee.com 链接, 此链接已失效
- 启用更新日志文件: update.log
- 更新 README
