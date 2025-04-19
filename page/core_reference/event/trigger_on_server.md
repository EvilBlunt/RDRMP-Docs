# event.trigger_on_server

![Client](https://img.shields.io/badge/Client-00FFFF)

Triggers an event, immediately invoking all associated handlers on the server side.

```lua
event.trigger_on_server(name --[[ string ]], ...)
```

---

#### 💡Example Usage

```lua
-- client.lua
-- Trigger an event called 'freeroam:give_money' from a specific client sent to the server.
event.trigger_on_server("freeroam:give_money", 1000)

-- server.lua
event.register("freeroam:give_money")
event.add_handler("freeroam:give_money", function(_client, _amount)

    print("A client ".._client.." asked to received: $".._amount)
end)
```