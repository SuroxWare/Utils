# SuroxWare Utils
Useful utils for roblox executors.

## How to use
1. Choose a script from the list below.
2. Copy the code block into your executor.
3. Adjust the variables (like _G values) if needed.
4. Execute and enjoy!

### Discord Invite Opener
```lua
-- Configurations
_G.Discord_Invite = "Your Invite" -- Replace with your invite.
_G.Discord_Debug  = true -- Set to true to see debug logs in the console.

-- Execute Script
loadstring(game:HttpGet("https://raw.githubusercontent.com/SuroxWare/Utils/refs/heads/main/discord"))()

-- Status Handling (returns: "Opened", "Copied" or "Failed")
local status = _G.Discord_Status
print("Discord Status:", status)
```

> **Notes**
> * You can use the full invite link or just the invite code.
> * Some Executors can't open Discord, in this case the full invite link will be copied.
> * If a executor doesnt support `setclipboard` then `_G.Discord_Status` will be **Failed**
> * `_G.Discord_Invite` will be cleared in the loadstring.
> * `_G.Discord_Status` is only available for **0.5s**.
