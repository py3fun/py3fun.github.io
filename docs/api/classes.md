# 类文档

API 中提供的核心类定义。

## 核心类

### `APIClient`

API 客户端类，用于与服务器通信。

**初始化参数:**
- `api_key` (str): API 密钥
- `base_url` (str): 基础 URL
- `timeout` (int, optional): 请求超时时间，默认 30 秒

**属性:**
- `is_connected` (bool): 连接状态
- `last_error` (str): 最后一次错误信息

**方法:**

#### `connect()`
建立连接。

**返回:** `bool` - 连接是否成功

#### `disconnect()`
断开连接。

#### `send_request(endpoint, data=None, method="GET")`
发送请求。

**参数:**
- `endpoint` (str): 请求端点
- `data` (dict, optional): 请求数据
- `method` (str): HTTP 方法

**返回:** `dict` - 响应数据

**示例:**
```python
client = APIClient(
    api_key="your-key",
    base_url="https://api.example.com"
)

if client.connect():
    response = client.send_request("/users", method="GET")
    print(response)
    client.disconnect()
```

### `DataProcessor`

数据处理器类。

**初始化参数:**
- `config` (dict): 处理器配置

**方法:**

#### `process(data)`
处理数据。

**参数:**
- `data` (Any): 待处理数据

**返回:** `dict` - 处理结果

#### `validate(data)`
验证数据。

**参数:**
- `data` (Any): 待验证数据

**返回:** `bool` - 验证结果

**示例:**
```python
processor = DataProcessor({
    "format": "json",
    "strict_mode": True
})

result = processor.process(raw_data)
```

### `ConfigManager`

配置管理器类。

**方法:**

#### `load_config(file_path)`
加载配置文件。

#### `get(key, default=None)`
获取配置值。

#### `set(key, value)`
设置配置值。

#### `save(file_path)`
保存配置到文件。

## 异常类

### `APIError`
API 相关错误的基类。

### `ConnectionError`
连接错误。

### `ProcessingError`
数据处理错误。

## 相关链接

- 返回 [API 概览](overview.md)
- 查看 [函数文档](functions.md)
