# 配置说明

如何配置和自定义你的环境。

## 配置文件

### 环境变量

```bash
export YOUR_APP_API_KEY="your-api-key"
export YOUR_APP_ENV="production"
```

### 配置文件

```yaml
# config.yaml
api:
  key: "your-api-key"
  endpoint: "https://api.example.com"
  
database:
  host: "localhost"
  port: 5432
  name: "mydb"
```

## 高级配置

更多配置选项请参考 [API 文档](../api/overview.md)。
