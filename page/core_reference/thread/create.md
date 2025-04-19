# thread.create

![Client](https://img.shields.io/badge/Client-00FFFF)

Create a new thread to run your code on.

> [!WARNING]
> Executing code directly at a root of a LUA script isn't recommended, you must be sure to always run your code inside a thread.

```lua
thread.create(handler --[[ function ]])
```

---

#### 💡Example Usage

```lua
thread.create(function()

    -- Stuff here will be ran at thread creation (Script start)

    while true do

        -- Stuff here will be ran every frame...

        thread.wait(0)
    end
end)
```