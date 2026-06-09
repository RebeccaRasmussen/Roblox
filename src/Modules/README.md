# Module Scripts

This folder contains **ModuleScripts** (Reusable code modules).

## What are Module Scripts?

Module scripts are reusable code libraries that can be used by both server and client scripts:
- Shared utility functions
- Custom class definitions
- Configuration settings
- Game systems (inventory, combat, etc.)

## Example Structure

```lua
-- Example: MathUtils.lua
local MathUtils = {}

function MathUtils.Round(number, decimals)
    local mult = 10^(decimals or 0)
    return math.floor(number * mult + 0.5) / mult
end

function MathUtils.Clamp(value, min, max)
    return math.max(min, math.min(max, value))
end

return MathUtils
```

## How to Use

```lua
-- In another script:
local MathUtils = require(game.ReplicatedStorage.MathUtils)
local rounded = MathUtils.Round(3.14159, 2) -- Returns 3.14
```

## Tips

- Module scripts must return a table or value
- Place them in `ReplicatedStorage` for shared access
- Keep modules focused on a single purpose
- Great for organizing complex code
