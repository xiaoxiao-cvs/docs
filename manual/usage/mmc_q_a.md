# 0.6.0版本更新Q&A

这个文件用来说明该次更新的问题

## 如何更新0.6.0 ❓
::: warning
- *不要*直接覆盖！

- *不要*pull后直接启动！

:::

-----------------------------------

- 你该怎么做：

    - 1.新建文件夹

    - 2.重新进行完整安装流程，参考教程[0.6.0版本部署教程](/manual/deployment/mmc_deploy_windows)

    - 3.**或者**使用[一键包](https://github.com/MaiM-with-u/MaiBot/releases/tag/EasyInstall-windows)

- 4.**如果**出现未知错误，删除原来数据库里 messages 和 chat_streams 中 所有内容

## 我原来的配置文件怎么办？

- 1.复制原来的bot_confg.toml

- 2.黏贴到0.6.0根目录的/config下，或者对照选项填入

- 3.启动0.6.0一次后，会生成一个.env文件。参考原来.env.prod的内容，填写0.6.0根目录下的.env

## 0.6.0版本以前的记忆会保存吗？

- 会

- 前提是不删除数据库的graph_data.edges 和 graph_data.nodes 

## 0.6.0版本以前的表情包怎么继承？

- 复制/data/emoji 到 0.6.0版本的/data/emoji

## 没run.bat吗？

- 没有，0.6.0使用了新的启动方式
- 如果你是手动部署：
    - 激活你的python环境，然后来到麦麦根目录，执行`python bot.py`
    - 然后启动napcat
    - 再启动搭载了插件的nonebot端

