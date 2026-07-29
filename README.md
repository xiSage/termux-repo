# termux-repo

个人 Termux APT 软件源，托管在 GitHub Pages 上。

## 添加源

在 Termux 中执行：

```bash
echo "deb [trusted=yes] https://xisage.com/termux-repo stable main" \
  > $PREFIX/etc/apt/sources.list.d/xisage.list

pkg update
```

## 安装软件包

```bash
pkg install hitokoto
```

## 可用软件包

| 包名 | 说明 |
|------|------|
| hitokoto | 一言 CLI —— 在终端中获取一条随机的一言句子 |

## 说明

- 源由 [hitokoto-cli](https://github.com/xiSage/hitokoto-cli) 的 CI 自动构建并发布。
- 如未签名，`[trusted=yes]` 是必须的。
