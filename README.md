# ZmyBot OpenAPI

这份目录只放 Apifox 用的接口文档。HTTP 和 WebSocket 都在 `openapi.yaml`。

接收人 `to_wxid` 可以是个人 wxid，也可以是群 id，群 id 以 `@chatroom` 结尾。

## 导入 Apifox

1. 打开 [Apifox](https://app.apifox.com)。
2. 进入项目，选择导入 OpenAPI/Swagger。
3. 数据源选 URL，填仓库里 `openapi.yaml` 的 raw 地址。
4. 导入后把 `/ws` 标成 WebSocket。客户端帧、回复帧和事件推送都写在该接口说明里。
5. 需要仓库更新后自动同步时，用 Apifox 的定时导入，地址仍是这份 `openapi.yaml`。

鉴权：`Authorization: Bearer <token>`、请求头 `x-api-token`，或查询参数 `access_token`。
