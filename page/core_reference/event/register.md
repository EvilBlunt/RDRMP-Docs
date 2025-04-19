# event.register

![Client](https://img.shields.io/badge/Client-00FFFF)
![Server](https://img.shields.io/badge/Server-00FFAA)

Register a new event that can be triggered later if at least one handler as been associated with it. Works on both client and server side.

> [!NOTE]
> It's safe to call multiple times, if it's already registered, the function will simply have no effect.

```lua
event.register(name --[[ string ]])
```

---

#### 💡Example Usage

```lua
event.register("freeroam:give_money") -- Register an event called 'freeroam:give_money' (You need to associate an handler later on)
```

> [!TIP]
> Our naming convention typically follows this pattern [resource_name]:[event_purpose]. That's why the example uses "freeroam:give_money". However, you're free to name it as you wish.