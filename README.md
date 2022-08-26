```lua
getgenv().Palette = Palette or loadstring(game:HttpGet("https://github.com/0zBug/EmojiPalette/blob/main/65794.lua?raw=true"))()

local function Emoji(r, g, b)
    return Palette[math.floor((bit32.lshift(r / 15, 16) + bit32.lshift(g / 0xF, 8) + b / 0xF) * 0xF / 0xFF + 1)]
end

print(Emoji(0, 0, 0)) --> ⬛
print(Emoji(255, 255, 255)) --> ⬜
print(Emoji(128, 0, 255)) --> 🍇
print(Emoji(255, 255, 0)) --> 🟨
```
