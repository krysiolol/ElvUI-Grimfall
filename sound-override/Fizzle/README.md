# Silent Fizzle Sounds

These five **empty** `.wav` files replace the WotLK 3.3.5a spell-fizzle sounds (cast failed) with silence:

- `FizzleFireA.wav`
- `FizzleFrostA.wav`
- `FizzleShadowA.wav`
- `FizzleHolyA.wav`
- `FizzleNatureA.wav`

## Why

The fizzle ("your spell failed") sound is played by the game client itself, not by the UI — so no addon can mute it with Lua in 3.3.5a. Overriding the sound files with empty ones is the only reliable way to silence it.

The **Error Text & Sound** option in `ElvUI_Enhanced` (see the main README) mutes the error *messages*, but the fizzle tick keeps playing. Drop these files in and the tick is gone too.

## Installation

Copy the `Fizzle` folder into your client's locale Sound folder. For English clients:

```
World of Warcraft\Data\enUS\Sound\Spells\Fizzle\
```

Replace `enUS` with your client locale if different:

| Locale | Folder |
| ------ | ------ |
| English | `enUS` |
| Spanish (Latin America) | `esMX` |
| French | `frFR` |
| German | `deDE` |
| Brazilian Portuguese | `ptBR` |
| Russian | `ruRU` |
| Korean | `koKR` |
| Simplified Chinese | `zhCN` |
| Traditional Chinese | `zhTW` |

## Uninstall

Delete the `Fizzle` folder from `Data\<locale>\Sound\Spells\` and the original sounds return.