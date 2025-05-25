# Controller Buttons

This is a full list of all the usable controller buttons.

## List
| Name | Image | Button |
| :----------- | :------: | :------: |
| TRIGGER_LEFT | ![LTRIGGER](../../assets/xbox_button_icons/B32aDhG.png) | 0 |
| TRIGGER_RIGHT | ![RTRIGGER](../../assets/xbox_button_icons/8fBZX5u.png) | 1 |
| BUMPER_LEFT | ![LB](../../assets/xbox_button_icons/cTjruGm.png) | 2 |
| BUMPER_RIGHT | ![RB](../../assets/xbox_button_icons/N6tGiDZ.png) | 3 |
| Y | ![Y](../../assets/xbox_button_icons/ymqhroT.png) | 4 |
| B | ![B](../../assets/xbox_button_icons/9qlEa0H.png) | 5 |
| A | ![A](../../assets/xbox_button_icons/0MgNhZs.png) | 6 |
| X | ![X](../../assets/xbox_button_icons/jMHzSOK.png) | 7 |
| BACK | ![BACK BUTTON](../../assets/xbox_button_icons/K8MY7XX.png) | 8 |
| STICK_LEFT | ![LSTICK](../../assets/xbox_button_icons/Tyv59XP.png) | 9 |
| STICK_RIGHT | ![RSTICK](../../assets/xbox_button_icons/y6XAou1.png) | 10 |
| START | ![START](../../assets/xbox_button_icons/9wTmr5n.png) | 11 |
| DPAD_UP | ![DPAD UP](../../assets/xbox_button_icons/g8GVkR6.png) | 12 |
| DPAD_RIGHT | ![DPAD RIGHT](../../assets/xbox_button_icons/EPioFjm.png) | 13 |
| DPAD_DOWN | ![DPAD DOWN](../../assets/xbox_button_icons/Zk4k6Jy.png) | 14 |
| DPAD_LEFT | ![DPAD LEFT](../../assets/xbox_button_icons/8KEeiDT.png) | 15 |

## Known Natives that use these buttons

| Native | Hash |
| :------------ | :------------: |
| natives.core.is_button_down | 0xC3297B50 |
| natives.core.is_button_pressed | 0x7BCB3F15 |
| natives.core.is_button_released | 0xB04EB731 |
| natives.core.get_analog_button_value | 0x23C9C74A |

## Snippet

```lua
BUTTON =
{
    NONE = -1,
    TRIGGER_LEFT = 0,
    TRIGGER_RIGHT = 1,
    BUMPER_LEFT = 2,
    BUMPER_RIGHT = 3,
    Y = 4,
    B = 5,
    A = 6,
    X = 7,
    BACK = 8,
    STICK_LEFT = 9,
    STICK_RIGHT = 10,
    START = 11,
    DPAD_UP = 12,
    DPAD_RIGHT = 13,
    DPAD_DOWN = 14,
    DPAD_LEFT = 15
}
```

---

#### 💡Example Usage

```lua
if natives.core.is_button_pressed(BUTTON.BUMPER_LEFT) then

    print("LB button has just been pressed!")
end
```