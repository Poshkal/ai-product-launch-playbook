---
name: ai-product-launch-playbook
description: "将AI产品想法收敛为可测MVP、评估试点准备或设计上线门禁时使用"
---

# AI 产品从想法到试点

## When to use

将AI产品想法收敛为可测MVP、评估试点准备或设计上线门禁时使用。

## Preconditions

确认输入、当前版本、可用工具及本次授权范围。历史案例只作方法依据，不能替代当前验证。缺少关键输入时先做可独立完成的只读检查，再列阻塞。

## Procedure

1. 定义用户、问题、现有替代、价值假设和可观察成功指标，不以项目名字证明验证成功。
2. 划分MVP、免费/付费权益、角色与数据边界，保留最小闭环。
3. 先读当前调用链与失败记录，将正常、无效输入、取消、重试、恢复与越权加入验收。
4. 将身份认证、支付确认与解锁绑定服务端事实；前端显示/上传成功不等于支付/审核/上线成功。
5. 在授权隔离环境试点并区分合成用户与真人反馈，给继续/暂停条件与回滚方案；发布单独授权。

## Tool permissions

需求/源码只读审计、隔离原型和本地测试；不创建付费订单、不迁移生产库、不提交审核。

## Failure handling

缺用户证据、支付闭环或必需权限则BLOCKED对应里程碑；确认缺陷NEED FIX。

## Deliverables

按下方输出契约交付本技能步骤中要求的清单、草稿/方案及证据；未执行项单列。

## Acceptance criteria

价值假设有验证方式；必需用户旅程、故障恢复、权限与支付各自有证据，缺项不能发布。

## Hard boundaries

不泄露密钥、客户隐私或非公开商业资料，不覆盖用户已有工作。读取权限不等于外发权限；生产变更按用户明确授权执行。

## Response contract

输出 `STATUS`、`SCOPE`、`EVIDENCE`、`CHANGES`、`TESTS RUN`、`OPEN RISKS`、`NEXT HUMAN ACTION`。逐项区分 PASS / NEED FIX / BLOCKED / NOT VERIFIED；历史记录、mock、本次本地与平台实测分列。

## Evidence and examples

阅读 [历史案例](references/cases.md) 时只加载与任务相关的案例；证据索引见其中链接。
