# frida-mogai

> [nosuke-server](https://github.com/Machao147258-max/huizong/tree/main/frida/%E9%AD%94%E6%94%B9frida) — 基于 Frida 17.11.0 源码魔改的反检测版 frida-server

本仓库存储大文件二进制，完整项目请见 **[huizong](https://github.com/Machao147258-max/huizong)**。

## 文件

| 文件 | 大小 | 说明 |
|:---|:---|:---|
| `nosuke-server` | 106MB | Android x86_64 魔改 frida-server |
| `nosuke-src.tar.gz` | 379MB | 魔改后的 frida-core 源码 |

## 使用

```bash
adb push nosuke-server /data/local/tmp/
adb shell su -c '/data/local/tmp/nosuke-server -l 0.0.0.0:31337 &'
frida -H 127.0.0.1:31337 -n 应用名
```

> 客户端版本需匹配 **Frida 17.11.0**
