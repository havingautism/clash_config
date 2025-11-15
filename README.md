配置文件介绍

本项目包含两个 Clash 配置文件，分别为 `clash_config_lite.yaml` 和 `clash_config_ultra.yaml`，适用于不同的使用场景和需求。以下是每个配置文件的详细介绍。

## 1. `clash_config_lite.yaml` - 轻量版配置文件

### 特点
- **轻量简洁**：适合PC端和手机端对规则颗粒度要求不高的用户。
- **基础功能**：包含常用的代理组和规则，满足日常使用需求，防止DNS泄露。

### 配置文件结构
- **代理组**：包含节点选择、流媒体节点、香港节点、台湾节点、狮城节点、日本节点、美国节点等。
- **规则**：支持国内外常用网站的分流，如 Google、Netflix、Telegram、Steam 等。
- **DNS 配置**：支持 fake-ip 模式，优化 DNS 解析速度。

### 使用说明
1. 下载 `clash_config_lite.yaml` 文件。
2. 在配置文件中填写自己的机场订阅地址。
3. 将配置文件导入 Clash 客户端即可使用。

---

## 2. `clash_config_ultra.yaml` - 增强版配置文件

### 特点
- **功能丰富**：只适合PC端对配置要求较高的用户，提供更细致的分流规则和代理组，性能开销更大。
- **高级 DNS 配置**：只保留H3 DNS配置，牺牲速度提高隐私和安全性。

### 配置文件结构
- **代理组**：包含节点选择、流媒体节点、香港节点、台湾节点、狮城节点、日本节点、美国节点等。
- **规则**：支持国内外常用网站的分流，如 Google、Netflix、Telegram、Steam 等，并在分流上增加更详细的匹配支持。
- **DNS 配置**：支持 DoH 和 H3 协议，提高 DNS 解析安全性。

### 使用说明
1. 下载 `clash_config_ultra.yaml` 文件。
2. 在配置文件中填写自己的机场订阅地址。
3. 将配置文件导入 Clash 客户端即可使用。

---

## 3. `clash_config_ultra_geosite.yaml` - geosite版配置文件（强烈推荐）

### 特点
- **功能丰富**：适合PC端手机端用户，提供细致的分流规则和代理组:
1. 完善TUN和DNS的逻辑，但是一般不建议开启，用系统代理模式就行
2. 优化geox-url
3. 优化health-check，补充max-failed-times，timeout，lazy: false的逻辑
4. 使用GeoSite而不是过时的rule-providers，可以节省大量RAM和检索时间

- **高级 DNS 配置**：新mihamo内核(1.18.10后)引入direct-nameserver，更精细的dns控制，无DNS泄露风险。


### 使用说明
1. 下载 `clash_config_ultra_geosite.yaml` 文件。
2. 在配置文件中填写自己的机场订阅地址。
3. 将配置文件导入 Clash 客户端即可使用。

## 贡献与反馈

如果你有任何建议或问题，欢迎提交 Issue 或 Pull Request。我们非常欢迎你的贡献！🚀



