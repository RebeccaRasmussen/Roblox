# Client Scripts

This folder contains **LocalScripts** (Scripts that run on the player's device).

## What are Local Scripts?

Local scripts run on each player's device and handle:
- User interface (GUI) interactions
- Camera controls
- Client-side effects and animations
- Input handling (keyboard, mouse, touch)

## Example Structure

```lua
-- Example: CameraShake.lua
local camera = workspace.CurrentCamera

local function shakeCamera()
    -- Add camera shake effect
    camera.CFrame = camera.CFrame * CFrame.Angles(
        math.rad(math.random(-5, 5)),
        math.rad(math.random(-5, 5)),
        0
    )
end
```

## Tips

- Local scripts run separately for each player
- They can't directly modify server data
- Use them for responsive UI and effects
- Put them in `StarterPlayer.StarterPlayerScripts` or `StarterGui` in Roblox Studio
- Use RemoteEvents to communicate with the server
