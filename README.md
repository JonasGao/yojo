# yojo

基于 YApi 对数据模型的描述，生成 Java 的 POJO 类。

描述形如：

```json
{
  "type": "object",
  "properties": {
    "comment": {
      "type": "string"
    },
    "email": {
      "type": "string",
      "description": "邮箱地址"
    }
  },
  "required": [
    "email"
  ]
}
```

生成

```java
class SomeUserTypedName {

    private String comment;

    private String email;

}
```