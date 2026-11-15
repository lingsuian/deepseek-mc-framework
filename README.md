# MC 模组服握手框架（DeepSeek MC 握手包）

让 mineflayer 系机器人接入 **Fabric / Forge 模组服**的底层框架。
原版协议客户端会在登录阶段被挡（Fabric 的登录期 channel、Forge 的 FML3 握手），这里补的就是那一层。

## 下载

| 包 | 说明 |
|---|---|
| `MC-handshake-framework-Fabric-v1.zip` | Fabric 版：登录 channel 应答、注册表同步、state 表与碰撞箱兜底；内含乌托邦 1.20.1 适配数据 |
| `MC-handshake-framework-Forge-v1.zip` | Forge 版：FML3 握手（1.18+），干净的握手层 |

解压即用，包内各带 README。

## 能做什么

- **进得去**：Fabric 登录期通道应答 / Forge FML3 握手
- **认得出**：接住 `fabric:registry/sync/direct`，模组方块、物品、实体有名字
- **走得动**：state 表注入 + 碰撞箱兜底，不会走错位，也不会让物理把宿主带崩
- **说清楚**：state id 需从整合包反推、哈希要和服务端一致，限制都写在包里 README

## 隐私

不含账号、密码、token、API key、cookie、个人昵称与服务器地址。已做整包扫描。

## 许可

未附许可证。转载/二次分发前请先联系作者。
