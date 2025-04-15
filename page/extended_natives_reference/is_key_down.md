# is_key_down `0xAC93D58A`

```lua
natives.extended.is_key_down(_keycode --[[ number/string ]])
```

---

#### 💡Example Usage

```lua
-- Using string keycode format
if natives.extended.is_key_down("F5") then

    print("F5 (Id 63) key has been pressed!")
end
```

```lua
-- Using number keycode format
if natives.extended.is_key_down(63) then

    print("F5 (Id 63) key has been pressed!")
end
```
