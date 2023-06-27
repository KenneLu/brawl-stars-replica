# Brawl Stars Replica | 《荒野乱斗》复刻项目
- EN
  - Brawl Starts game's replica demo, tests passing on UE4.26 blueprint.
  - Introduction video: https://www.bilibili.com/video/BV1Au411e7jw/
  - Documents: https://www.zhihu.com/column/c_1652093990043394048
- CN
  - 基于 UE4.26 纯蓝图开发的《荒野乱斗》手游复刻项目。
  - 介绍视频：https://www.bilibili.com/video/BV1Au411e7jw/
  - 介绍文档：https://www.zhihu.com/column/c_1652093990043394048

# Content | 游戏内容
1. Hero Type | 英雄类型
- Colt | 柯尔特
- Nita | 妮塔
- Primo | 普里莫
- Shelly | 雪莉
2. Game Mode | 游戏模式
- Gem Grab | 宝石争霸
- Heist | 金库攻防
3. Online | 联机
- LAN | 局域网（WiFi）
- Steam | 广域网（Steam 服务器）

# Platform | 运行平台
- PC ( Windows ) | 电脑（Windows 系统）

# Editor / Plugins | 引擎 / 插件
- Visual Studio 2019 | VS 2019（UE4.26 最高只支持到 2019）
- Unreal Engine 4.26 | 虚幻引擎 4.26
- Advance Session 4.26 | 高级会话插件 4.26
- Advance Steam Session 4.26 | 高级 Steam 会话插件 4.26

# Quick Debug | 快速上手调试
- EN
  - Movement: W A S D.
  - Attack: Mouse button. Left button release normal skill, right one release ultimate skill.
  - Aiming: Hold down the mouse button, then move mouse toward the enemy.
  - Login Level: Map/Login/LoginStart/L_LoginStart
  - Team Level: Map/Login/LoginRoom/L_LoginRoom
  - Gem Grab Game Level: Map/Game/GemGrab/L_GemGrab
  - Heist Game Level：Map/Game/Heist/L_Heist
  - Switch Hero in Game Level: Goto PlayerController in [Map/Base/Blueprint/PC_GameBase], find evnet [ClientGetHeroTypeAndSpawn], then change defualt [SET HeroType] node.
  - Stop AI Spawn in Game Level: Goto GameMode in [Map/Base/Blueprint/GM_GameBase], find event [GameBegin], then remove [SpawnAI] node.
- CN
  - 角色移动：键盘 W A S D 控制角色上下左右。
  - 角色攻击：鼠标左键释放普攻，右键释放大招。
  - 攻击瞄准：按住鼠标键不放，然后朝敌人方向拖动。
  - 【大厅】地图：Map / Login / LoginStart / L_LoginStart
  - 【小队】地图：Map / Login / LoginRoom / L_LoginRoom
  - 《宝石争霸》关卡：Map / Game / GemGrab / L_GemGrab
  - 《金库攻防》关卡：Map / Game / Heist / L_Heist
  - 关卡内切换英雄：在 Map / Base / Blueprint / PC_GameBase 的事件图表，其中的【ClientGetHeroTypeAndSpawn】事件，修改默认的【SET HeroType】节点即可。
  - 停止 AI 的生成：在 Map / Base / Blueprint / GM_GameBase 的事件图表，其中的【GameBegin】事件，移除【SpawnAI】节点即可。
