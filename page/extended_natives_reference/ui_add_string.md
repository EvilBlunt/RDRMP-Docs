# ui_add_string `0x5D425448`

Add or override a GXTEntry (It can be used to replace existing game text or simply register a newly GXTEntry key).

```lua
natives.extended.ui_add_string(_gxtentry --[[ string ]])
```

---

#### 💡Example Usage

```lua

-- This code will create a blip in coords (0,0,0) with the name 'Hello World!'

-- Registering the custom GXTEntry
natives.extended.ui_add_string("THIS_IS_A_CUSTOM_GXTENTRY", "Hello World!")

-- Create our blip and name it using the GXTEntry
local myblip = natives.hud.add_blip_for_coord(vector3(0.0, 0.0, 0.0), 396, 0.0, 2, 0)
natives.hud.set_blip_name(myblip, "THIS_IS_A_CUSTOM_GXTENTRY")

```
