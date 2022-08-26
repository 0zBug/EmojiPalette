# 65794
```lua
math.floor((bit32.lshift(r / 0xF, 16) + bit32.lshift(g / 0xF, 8) + b / 0xF) * 0xF / 0xFF + 1)
```
# 256
```lua
bit32.bor(bit32.bor(bit32.lshift(math.round(r / 0xFF * 7), 5), bit32.lshift(math.round(g / 0xFF * 7), 2)), math.round(b / 0xFF * 3)) + 1
```
