# event.trigger

![Client](https://img.shields.io/badge/Client-00FFFF)
![Server](https://img.shields.io/badge/Server-00FFAA)

Triggers an event, immediately invoking all locally associated handlers.

```lua
event.trigger(name --[[ string ]], ...)
```

---

#### 💡Example Usage

```lua
-- Trigger an event called 'freeroam:give_money' with an amount of 1000$
event.trigger("freeroam:give_money", 1000)
```