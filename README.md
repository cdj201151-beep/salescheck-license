# SalesCheck 授权发码机

销售核对客户端的授权码签发界面（Ed25519 签名，纯前端、离线可用）。

## 重要

- **本仓库不含私钥，也不应包含私钥。** 没有 `private_key.pem` 就无法签出任何授权码。
- 私钥只在你本机 `~/.salescheck_license/private_key.pem`，通过页面上的「选择文件」读入浏览器内存，不会上传。
- 请不要把私钥、`.sclic`、任何 `*.pem` 提交到这个仓库；`.gitignore` 已做拦截。

## 公钥指纹

`FF5224DA…0BDF` —— 与客户端 `license_core.py` 内置公钥一致。

## 用法

打开页面 → 载入 `private_key.pem` → 填设备号与天数 → 生成 → 复制。
