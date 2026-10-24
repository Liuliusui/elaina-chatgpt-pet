# 伊蕾娜 · ChatGPT Pet

《魔女之旅》灰之魔女伊蕾娜的 Q 版动态宠物素材。银发、紫瞳、粉紫帽带与黑紫色长袍，包含 9 种基础动作和 16 个视线方向，共 73 帧。

<p>
  <img src="previews/all-states.gif" width="192" height="208" alt="伊蕾娜基础动作预览">
  <img src="previews/look-directions.gif" width="192" height="208" alt="伊蕾娜16个视线方向预览">
</p>

## 下载

- [透明精灵图 spritesheet.png](spritesheet.png)：完整的清晰修复版素材。
- [动画参数 pet.json](pet.json)：帧尺寸、行顺序、时长与视线方向。
- [基础动作预览](previews/all-states.gif) · [视线预览](previews/look-directions.gif) · [待机与跳跃衔接](previews/idle-jump-idle.gif)。
- 下载整个项目：点击 GitHub 的 **Code → Download ZIP**。

## 素材规格

| 项目 | 数值 |
| --- | --- |
| 图片格式 | 带透明通道的 PNG |
| 精灵图尺寸 | 1536 × 2288 px |
| 网格 | 8 列 × 11 行 |
| 单帧尺寸 | 192 × 208 px |
| 精灵版本 | v2 |
| 有效帧数 | 73，未使用的格子保持透明 |

本仓库保存了修复过度去色处理后的版本，恢复银发、帽檐和衣边的线条。单帧分辨率仍为 192 × 208；放大显示时，细节会受到这个分辨率限制。

## 动作顺序

行号与列号从 0 开始，有效帧从每行最左侧排列。每帧时长见 `pet.json`。

| 行 | 状态 | 帧数 | 动作 |
| --- | --- | --- | --- |
| 0 | `idle` | 6 | 待机、呼吸与眨眼 |
| 1 | `running-right` | 8 | 向右跑动 |
| 2 | `running-left` | 8 | 向左跑动 |
| 3 | `waving` | 4 | 挥手 |
| 4 | `jumping` | 5 | 轻跳与落地 |
| 5 | `failed` | 8 | 失落与恢复 |
| 6 | `waiting` | 6 | 等待输入或确认 |
| 7 | `running` | 6 | 思考与工作 |
| 8 | `review` | 6 | 检查结果 |
| 9 | `look-directions-a` | 8 | 0° 至 157.5° |
| 10 | `look-directions-b` | 8 | 180° 至 337.5° |

视线采用屏幕坐标：0° 向上、90° 向右、180° 向下、270° 向左，按顺时针每 22.5° 一帧。`running` 表示正在工作或思考，与左右跑动状态分开。

## 使用素材

下载 `spritesheet.png` 与 `pet.json`，用于备份、动画查看，或接入支持上述网格布局的宠物播放器。读取某一帧时，裁剪区域为 `(列 × 192, 行 × 208, 192, 208)`，并按对应时长播放。

GitHub 保存的是素材文件；账户里的宠物记录与这个仓库分开管理。仓库中的 `pet.json` 是素材说明，不包含个人账户的宠物 ID。

## 角色与制作

角色为《魔女之旅》的伊蕾娜。[角色资料](https://zh.moegirl.org.cn/%E4%BC%8A%E8%95%BE%E5%A8%9C)。本项目为 AI 辅助制作的同人宠物素材，相关原作与角色权利归各自权利人所有。
