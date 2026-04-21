# 聊天记录导入知识库（Sanhe V2）

本目录用于存放从历史聊天记录中提炼的业务知识。

## 核心原则

- 不直接把聊天原文当知识库主内容
- 先清洗，再归类，再提炼，再入库
- 保留来源、时间范围、适用范围与可信度说明
- 私人信息、纯情绪表达、未确认判断、与业务无关内容不直接入库
- 新资料优先判断：主干 / 支线 / 低信号，不再无序堆积
- 凡是主公新增交付的三禾聊天资料，默认按现有 V2 结构做增量补位，不得把单批新资料当成重新定义 sanhe-ops 架构的起点
- 先查现有结构，再判断层级，再决定落点；优先补充已有 playbook / rules / index，只有现有结构确实接不住时才新开文件
- 新资料进入知识库时，必须交代：补到了哪一层、补进了哪些已有文件、哪些内容只保留为背景或低信号索引

## 当前主干知识层（6个板块）

| 目录 | 主题 | 核心文件 |
|------|------|---------|
| `ops/` | 打包发货与异常处理 | packaging-shipping-playbook.md（含案例卡） |
| `operations-systems/` | 门店系统/档口/旧货时效 | yidiantong / stall-collab / old-stock-expiry |
| `social-commerce/` | 社媒执行与电商联动 | social-commerce-playbook / content-rules |
| `commerce/` | 电商基础执行与利润感 | commerce-ops-basics-v1.md |
| `business-trade/` | 业务经营与供应侧 | business-trade-playbook-v1.md |
| `campaigns/` | 专项冲刺（喜糖/礼盒/节点） | xitang-sprint-playbook-v1.md |

## 支线参考层
- `side-projects/`：品牌/视觉协作，不混入主营

## 低信号原始索引层
- `raw-index/`：已查看但暂不升格的低信号或非业务资料

## 入口文件
- 结构总览：`STRUCTURE-V2.md`
- 快查索引（按问题类型定位文件）：`INDEX.md`
- 核心规则卡（可直接调用）：`rules-core-v1.md`

## 当前文件清单（共19个md，不含子目录README）

**主干（13个）**
- ops/packaging-shipping-playbook.md
- operations-systems/yidiantong-operations-playbook-v1.md
- operations-systems/stall-collab-playbook-v1.md
- operations-systems/old-stock-expiry-playbook-v1.md
- social-commerce/social-commerce-playbook-v1.md
- social-commerce/content-rules-v1.md
- commerce/commerce-ops-basics-v1.md
- business-trade/business-trade-playbook-v1.md
- campaigns/xitang-sprint-playbook-v1.md
- rules-core-v1.md（规则调用层）

**支线（1个）**
- side-projects/animore-brand-collab-v1.md

**索引（3个）**
- raw-index/private-chat-low-signal-index.md
- raw-index/private-chat-batch2-index.md

**结构说明（2个）**
- README.md（本文件）
- STRUCTURE-V2.md

## 当前状态

已完成：
- 结构层定义（V2）
- 主干知识完整导入（6个板块）
- 核心规则卡抽取（35条规则 + 4条原则）
- 重复内容合并（cases/ 并入 ops/，early-margin 并入 commerce/）
- 新增私聊二轮筛查

进行中：
- 新增高信号私聊提炼（档口FL等）

已完成（2026-04-18）：
- 档口FL提炼（stall-fl-playbook-v1.md）
- 三禾行哆啦A梦兰姐提炼（store-lanjie-playbook-v1.md）
- 三禾行欣提炼（store-xin-packaging-playbook-v1.md）
- 档口Lucky_彤提炼（store-lucky-stall-playbook-v1.md）
- 三禾行Yan提炼（yan-onboarding-playbook-v1.md）
