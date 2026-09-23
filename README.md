# ZmyBot

本机 `http://127.0.0.1:58080`。请求头 `Authorization: Bearer <token>`。

接收人可以是好友 wxid，也可以是群 id（`xxx@chatroom`）。

| 接口 | 作用 |
| --- | --- |
| `POST /send_image` | 发图片。`robot_wxid`、`to_wxid`、`path` |
| `POST /send_private_msg` | 发好友文字 |
| `POST /send_group_msg` | 发群文字 |
| `WS /ws` | 同样的动作，外加事件推送 |

Apifox 导入地址：

`https://raw.githubusercontent.com/subisle/zmybot-openapi/main/openapi.yaml`
