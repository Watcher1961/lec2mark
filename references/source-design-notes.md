> 以下保留设计参考的来源归属，不表示分发上游文件或获得上游背书。发布时未逐一复查上游全部文件与历史版本。

# 外部 Skill 参考与本次取舍

设计阶段参考以下仓库的 SKILL.md。它们是本 Skill 的设计参考，不是后续执行时需要加载的依赖，也不代表上游的全部规则已被采纳。下述为重新表述的设计归纳，没有复制模板、脚本或示例正文。

| 已核对来源 | 借鉴到本 Skill 的内容 | 取舍 |
|---|---|---|
| [AL1S12/study-notes-generator](https://github.com/AL1S12/study-notes-generator/blob/master/SKILL.md) | 多文件去重、跨章节连接、保留公式和教师补充、增量融入已有笔记 | 不继承自动安装依赖；识别失败先回查原页，不把推测图意或公式当作已核实内容 |
| [siluy/obsidian-study-notes-skill](https://github.com/siluy/obsidian-study-notes-skill/blob/main/SKILL.md) | 总览与章节笔记、wikilinks、callouts、图示和带解释的例题 | 保留原 Skill 的概念教学顺序；不强制每章导图、固定题量或模式确认，不承诺考试结果 |
| [Shass27/stem-notes](https://github.com/Shass27/stem-notes/blob/main/SKILL.md) | 图像页视觉核对、来源页码与题号、数值验算、公布与原答案的差异 | 输出维持 Obsidian Markdown，不移植 LaTeX 输出流程及多轮选择问卷 |
| [LuoHaomin/study-notes](https://github.com/LuoHaomin/study-notes/blob/main/SKILL.md) | 长文语义分段再合成、处理进度、同章多文件融合、课程总览 | 不继承固定 token 阈值、按行数判定完成、每章强制新会话或每章等待确认 |

字幕对齐、无时间戳定位、手写指代与可信度、课程代码的理论映射是针对本次实际输入组合新增的规则，不宣称四个上游项目已提供完整实现。多来源处理规则与教材分析作为参考保留；合并后的教学组织以 SKILL.md 为准。

Obsidian 格式参照官方说明：[内部链接](https://help.obsidian.md/Linking+notes+and+files/Internal+links)、[提示框与折叠语法](https://help.obsidian.md/Editing+and+formatting/Callouts)。采用原生能力；链接、图像和公式仍应按实际产物验证。
