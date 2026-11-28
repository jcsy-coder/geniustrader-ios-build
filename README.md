# GeniusTrader 构建镜像

这个仓库里**没有源码**，只有加密后的 `payload.part*` 分片。
构建时在一次性 macOS runner 上用仓库 Secret `MIRROR_KEY` 解密再编译，
明文只存在于那次运行里，跑完即销毁。

由主仓库的同步脚本单向推送，**不要在这个仓库改任何东西**。
