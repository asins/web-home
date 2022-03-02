# Asins网家构建项目

构建项目基于zola创建

## 模板主题
目前使用 [blow](https://www.getzola.org/themes/blow/)

```bash
# 更新模板文件
git submodule add -b main git@github.com:tchartron/blow.git themes/blow
```
## 构建项目

```bash
# 构建项目内的内容
zola build

# 绑定静态网站项目
git submodule add -b master git@github.com:asins/asins.github.io.git public

# 构建子项目: Rust 语言备忘清单
zola --config ./config.toml build --output-dir ${RootPath}/public/rust-language-cheat-sheet
```
