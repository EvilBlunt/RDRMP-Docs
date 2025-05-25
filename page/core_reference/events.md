# 📃 Events

Below you will find a list of all the 'core' events used by RDRMP LUA API.

| Event Name | Client | Server |
| :------------ | :------------: | :------------: |
| core:on_resource_start | ✅ Yes | ❌ No |
| core:on_resource_stop | ✅ Yes | ❌ No |
| core:on_player_joined | ✅ Yes | ✅ Yes |
| core:on_player_left | ✅ Yes | ✅ Yes |
| core:on_chat_open | ✅ Yes | ❌ No |
| core:on_chat_close | ✅ Yes | ❌ No |
| core:on_chat_command | ❌ No | ✅ Yes |

---

#### 💡Example Usage

```lua
event.add_handler("core:on_resource_start", function(_name)

    if _name == CURRENT_RESOURCE_NAME then

        print("Resource ".._name.." has just been started !")
    end
end)
```

```lua
event.add_handler("core:on_resource_stop", function(_name)

    if _name == CURRENT_RESOURCE_NAME then

        print("Resource ".._name.." has just been stopped !")
    end
end)
```

```lua
-- Client definition
event.add_handler("core:on_player_joined", function(_client, _name, _islocal)

    print("Player ".._name.." has just joined the game !")
end)

-- Server definition
event.add_handler("core:on_player_joined", function(_client, _name)

    print("Player ".._name.." has just joined the game !")
end)
```

```lua
-- Client definition
event.add_handler("core:on_player_left", function(_client, _name, _islocal)

    print("Player ".._name.." has just left the game !")
end)

-- Server definition
event.add_handler("core:on_player_left", function(_client, _name)

    print("Player ".._name.." has just left the game !")
end)
```

```lua
event.add_handler("core:on_chat_open", function()

    print("Chat box has been opened !")
end)
```

```lua
event.add_handler("core:on_chat_close", function()

    print("Chat box has been closed !")
end)
```

```lua
event.add_handler("core:on_chat_command", function(_client, _command, _args)

    print("Chat command ".._command.." with parameters ".._args.." has been sent by client ".._client)
end)
```