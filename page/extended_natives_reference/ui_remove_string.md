# ui_remove_string `0x9173F8FE`

Remove a previously registered GXTEntry if there is one.

> [!WARNING]
> This doesn't unregister existing game GXTEntry, only the one added using 'ui_add_string'

```lua
natives.extended.ui_remove_string(_gxtentry --[[ string ]])
```