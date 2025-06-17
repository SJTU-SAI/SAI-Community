# 网站本地运行

官方教程：[Getting Started](https://squidfunk.github.io/mkdocs-material/getting-started/)

下面提供极简版教程：

## 安装依赖

我们所有的依赖安装都使用`pip`实现，请务必保证你的电脑里面安装了 pip[^1] 和 Python ，并且可以正常工作。当然，我们也推荐conda或者其他方式创造隔离环境(Python 3.12)。

- 克隆本仓库

```bash
git clone https://github.com/SJTU-SAI/SAI-Community.git
cd SAI-Community
```

- 安装依赖

```bash
pip install -r requirements.txt
```

安装完成后运行：

```bash
mkdocs --version
```
如果输出版本号说明安装成功。

## 运行网站

```bash
mkdocs serve
```

![Run Locally](https://s1.imagehub.cc/images/2025/06/13/68166482f41c7ab2bf1c60a3e32d25ad.png)

说明此时网页在本地渲染成功！浏览器中打开`http://127.0.0.1:8000/SAI-Community`即可，然后翻到对应修改的页面修改内容是否符合预期。

[^1]: [pip](https://pypi.org/project/pip/)