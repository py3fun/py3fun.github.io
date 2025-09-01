# 函数文档

API 中提供的核心函数说明。

## 核心函数

### `initialize(config)`

初始化应用程序。

**参数:**
- `config` (dict): 配置字典

**返回:**
- `bool`: 初始化是否成功

**示例:**
```python
config = {
    "api_key": "your-key",
    "endpoint": "https://api.example.com"
}
success = initialize(config)
```

### `process_data(data, options=None)`

处理输入数据。

**参数:**
- `data` (Any): 要处理的数据
- `options` (dict, optional): 处理选项

**返回:**
- `dict`: 处理结果

**异常:**
- `ValueError`: 数据格式不正确
- `ProcessingError`: 处理过程中出错

**示例:**
```python
result = process_data(
    data={"key": "value"},
    options={"format": "json"}
)
```

### `validate_input(input_data)`

验证输入数据的有效性。

**参数:**
- `input_data` (dict): 待验证的数据

**返回:**
- `tuple`: (is_valid: bool, errors: list)

**示例:**
```python
is_valid, errors = validate_input(user_data)
if not is_valid:
    print("验证失败:", errors)
```

## 工具函数

### `format_response(data, status="success")`

格式化 API 响应。

**参数:**
- `data` (Any): 响应数据
- `status` (str): 状态码

**返回:**
- `dict`: 格式化的响应

## 相关链接

- 返回 [API 概览](overview.md)
- 查看 [类文档](classes.md)
