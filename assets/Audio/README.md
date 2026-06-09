# Audio

This folder is for organizing information about sound effects and music used in your games.

## Audio in Roblox

Audio includes:
- Background music
- Sound effects (footsteps, explosions, etc.)
- Ambient sounds
- UI sounds (button clicks, notifications)

## Using Audio

```lua
-- Example: Playing a sound
local sound = Instance.new("Sound")
sound.SoundId = "rbxassetid://1234567890" -- Asset ID
sound.Volume = 0.5
sound.Parent = workspace
sound:Play()
```

## Finding Audio

- [Roblox Creator Marketplace - Audio](https://create.roblox.com/marketplace/audio)
- Upload your own sounds (Roblox Premium required for private audio)
- Use Roblox's library of free sounds

## Tips

- Keep track of Asset IDs for sounds you use
- Test volume levels - not too loud!
- Use appropriate sounds for different game events
- Consider adding a volume control for players
- Always respect copyright - only use sounds you have permission to use

## Audio Properties

- `Volume`: How loud (0 to 1)
- `Looped`: Whether to repeat
- `PlaybackSpeed`: How fast to play
- `TimePosition`: Where in the sound to start
