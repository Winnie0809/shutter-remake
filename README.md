# 透气窗重做资料 Skill

用于 Codex 的中文技能：指定订单12列汇总、Damage Report提取和中英对照Excel整理。可分别执行或一起执行。

## 使用

将本仓库中的 `shutter-remake` 文件夹复制到本机 Codex 的 skills 目录（通常为 `~/.codex/skills/`），然后在支持技能的会话中调用：

```text
请用 $shutter-remake 处理当前目录的售后资料：
递归生成 Damage Report 中英对照；
订单汇总只处理我在本次消息提供的订单号：……
```

也可以只请求其中一个流程。实际运行需要环境具有对应格式的读写工具；PDF、图片可能需要OCR。技能提供处理规范，不附带客户数据，也不承诺环境中已安装所有工具。

## 文件

- `shutter-remake/SKILL.md`：技能入口和范围规则。
- `shutter-remake/references/order-summary.md`：订单匹配、12列格式、日期和异常规则。
- `shutter-remake/references/damage-report.md`：报告范围、翻译术语、单元格和保存规则。

上传GitHub时只上传本文件所在目录的内容。技能包不包含真实订单、客户名称、业务附件、输出报表或聊天记录。所有结果另存，不覆盖原始文件；上传仓库和发布操作由使用者自行完成。
