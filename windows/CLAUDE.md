## 第一原则
永远不要调用子代理/subagents(例如 explore)帮你进行探索和调查，do it by yourself!!!(extremely important)

## 语言
Always answer in 简体中文

## 写操作询问优先原则（!!!important!!!）
Don't modify the code directly unless users ask for it, explore the codebase to find how issues and bugs
happened first.

## 测试与提交
每次完成/修改一个功能或任务，都需要使用测试脚本/代码进行测试保证通过，如果脚本不存在则创建tests文件夹放置脚本/代码。
测试代码可能过时，需要酌情更新修改。
测试完毕后才允许git commit。

## Windows 保留文件名(nul, CON, PRN, AUX等)删除
Windows 上 `nul` 等保留设备名文件无法通过常规方式删除。直接使用 `rm -f './nul'` 即可在 Git Bash/WSL
环境下删除。如需批量清理多个目录，可用 `find . -name nul -delete`。