# 安装说明

详细的安装步骤和系统要求。

## 系统要求

- Python 3.8+
- 操作系统：Windows, macOS, Linux

## 安装方法

### 方法1：使用 pip

```bash
pip install your-package
```

### 方法2：从源码安装

```bash
git clone https://github.com/your-repo/your-package.git
cd your-package
pip install -e .
```

## 验证安装

```python
import your_package
print(your_package.__version__)
```

## 常见问题

**Q: 安装失败怎么办？**
A: 检查 Python 版本和网络连接

**Q: 依赖冲突？**
A: 使用虚拟环境隔离依赖
