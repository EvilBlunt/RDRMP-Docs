# thread.wait

![Client](https://img.shields.io/badge/Client-00FFFF)

Wait the current thread. (Value in milliseconds)

```lua
thread.wait(ms --[[ number ]])
```

---

#### 💡Example Usage

```lua
thread.create(function()

    -- Execute a code here...

    thread.wait(5000) -- Wait 5 sec

    -- Execute an other code here...
end)
```