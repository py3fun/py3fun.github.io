# API 概览

API 接口的总体介绍和使用方法。

## 认证

所有 API 请求都需要包含 API Key：

```bash
Authorization: Bearer YOUR_API_KEY
```

## 基础 URL

```
https://api.example.com/v1
```

## 响应格式

所有响应都是 JSON 格式：

```json
{
  "success": true,
  "data": {...},
  "message": "操作成功"
}
```

## 错误处理

```json
{
  "success": false,
  "error": "错误代码",
  "message": "错误描述"
}
```

## 下一步

- 查看 [函数文档](functions.md)
- 了解 [类定义](classes.md)
