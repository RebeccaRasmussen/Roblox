# Server Scripts

This folder contains **ServerScripts** (Scripts that run on the Roblox server).

## What are Server Scripts?

Server scripts run on the Roblox server and handle:
- Game logic that needs to be secure
- Player data and stats
- Game state management
- Anti-cheat systems
- Leaderboards

## Example Structure

```lua
-- Example: WelcomeMessage.lua
local Players = game:GetService("Players")

Players.PlayerAdded:Connect(function(player)
    print(player.Name .. " has joined the game!")
end)
```

## Tips

- Server scripts can access everything in the game
- They are more secure than client scripts
- Use them for important game mechanics
- Put them in `ServerScriptService` in Roblox Studio
