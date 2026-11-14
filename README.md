# 贴吧签到Github Action版

自用留存，二次修改添加PushPlus 通知，本源fork自czp0312/TieBaSign

## 使用说明

1. Fork 本仓库，然后点击你的仓库右上角的 `Settings` -> `Secrets and variables` -> `Actions` 这一项，添加一个`Repository secrets`，变量名称为 `BDUSS`，支持同时添加多个帐户，BDUSS 之间用 `#` 隔开即可。

2. 设置好环境变量后点击你的仓库上方的 `Actions` 选项，第一次打开需要点击 `I understand...` 按钮，确认在 Fork 的仓库上启用 GitHub Actions 。

3. 任意发起一次commit，可以参考下图流程修改 `README.md` 文件。

- 打开`README.md`，点击 `Edit` 编辑按钮
- 修改任意内容，这里在末尾插入了空格，移动到最下面，点击提交

4. 至此自动签到就搭建完毕了，可以再次点击`Actions`查看工作记录，如果有`Baidu Tieba Auto Sign`则说明workflow创建成功了，点击右侧记录可以查看详细签到情况。

5.需要PushPlus 通知即重复第一步操作，添加一个`Repository secrets`，变量名称为 `PUSH_PLUS_TOKEN`
