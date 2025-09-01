# 实例代码

这里提供了完整的代码示例和使用案例。

## 基础示例

### Hello World

```python
def hello_world():
    """简单的问候函数"""
    return "Hello, World!"

if __name__ == "__main__":
    print(hello_world())
```

### 配置文件读取

```python
import yaml

def load_config(config_file):
    """加载配置文件"""
    with open(config_file, 'r', encoding='utf-8') as f:
        config = yaml.safe_load(f)
    return config

# 使用示例
config = load_config('config.yaml')
print(config['api']['endpoint'])
```

## 高级示例

### 异步处理

```python
import asyncio
import aiohttp

async def fetch_data(url):
    """异步获取数据"""
    async with aiohttp.ClientSession() as session:
        async with session.get(url) as response:
            return await response.json()

# 批量处理
async def process_urls(urls):
    tasks = [fetch_data(url) for url in urls]
    results = await asyncio.gather(*tasks)
    return results
```

### 错误处理

```python
import logging

logger = logging.getLogger(__name__)

def safe_operation(data):
    """带错误处理的安全操作"""
    try:
        result = complex_calculation(data)
        logger.info(f"操作成功: {result}")
        return result
    except ValueError as e:
        logger.error(f"数值错误: {e}")
        return None
    except Exception as e:
        logger.error(f"未知错误: {e}")
        raise
```

## 完整项目示例

查看我们的 [GitHub 仓库](https://github.com/py3fun/py3fun.github.io) 获取完整的项目代码。

## 相关链接

- 返回 [基础教程](basic-tutorial.md)
- 查看 [高级教程](advanced-tutorial.md)
- 参考 [API 文档](../api/overview.md)
