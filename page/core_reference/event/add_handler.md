# event.add_handler

![Client](https://img.shields.io/badge/Client-00FFFF)
![Server](https://img.shields.io/badge/Server-00FFAA)

Add an handler for a previously registered event. Works on both client and server side.

> [!TIP]
> You can associate multiple handlers to a single event.

```lua
event.add_handler(name --[[ string ]], handler --[[ function ]])
```

---

#### 💡Example Usage

```lua
event.add_handler("freeroam:give_money", function(_amount) -- Add an handler for the event 'freeroam:give_money' (Need to be registered first)

    print("Amount given: ".._amount)
end)
```

> [!TIP]
> Our naming convention typically follows this pattern [resource_name]:[event_purpose]. That's why the example uses "freeroam:give_money". However, you're free to name it as you wish.