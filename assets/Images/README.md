# Images

This folder is for organizing textures, decals, and UI images used in your games.

## Image Types in Roblox

1. **Decals**: Images displayed on surfaces
2. **Textures**: Wrap around parts
3. **UI Images**: Used in GUIs (buttons, icons, backgrounds)

## Using Images

```lua
-- Example: Adding a decal to a part
local decal = Instance.new("Decal")
decal.Texture = "rbxassetid://1234567890"
decal.Face = Enum.NormalId.Front
decal.Parent = game.Workspace.Part
```

## Image Requirements

- **Format**: PNG, JPG, or BMP
- **Size**: Max 1024x1024 pixels (recommended)
- **Upload**: Through Roblox Studio or website

## Finding Images

- Create your own using image editing software
- [Roblox Creator Marketplace - Decals](https://create.roblox.com/marketplace/decals)
- Use free texture websites (with proper licensing)

## Tips

- Keep images under 1MB for faster loading
- Use transparent PNGs for UI elements
- Name images descriptively
- Keep track of Asset IDs
- Test how images look in-game
- Respect copyright - only use images you have rights to use

## Common Uses

- Game logos and branding
- UI buttons and icons
- Posters and signs
- Part textures
- Skybox images
