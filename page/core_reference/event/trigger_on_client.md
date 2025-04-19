# event.trigger_on_client

![Server](https://img.shields.io/badge/Server-00FF2C)

Triggers an event, immediately invoking all associated handlers on the client side.

```lua
event.trigger_on_client(name --[[ string ]], client --[[ number ]], ...)
```

---

#### 💡Example Usage

```lua
-- server.lua
-- Trigger an event called 'freeroam:give_money' from the server, sending $1000 to a specific client.
-- (Passing -1 as the target will broadcast the event to all clients.)
event.trigger_on_client("freeroam:give_money", -1, 1000)

-- client.lua
event.register("freeroam:give_money")
event.add_handler("freeroam:give_money", function(_amount)

    print("The server has sent you: $".._amount)
end)
```