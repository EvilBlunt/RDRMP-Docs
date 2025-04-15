# is_key_released `0x21B6EB31`

Checks if a key has just been released. You can find the list of usable keycodes [here](https://docs.rdrmp.redmods.com/#/page/game_reference/keyboard_keycodes).

> [!TIP]
> This function supports two input types: a numeric keycode or a string representation of the key (e.g. "F5" or 63).

```lua
natives.extended.is_key_released(_keycode --[[ number/string ]])
```

---

#### 💡Example Usage

```lua
-- Using a string representation
if natives.extended.is_key_pressed("F5") then

    print("F5 (Id 63) key has just been released!")
end
```

```lua
-- Using a numeric keycode
if natives.extended.is_key_pressed(63) then

    print("F5 (Id 63) key has just been released!")
end
```
