# SuroxWare Utils
Useful utils for roblox executors.

## How to use
1. Choose a script from the list below.
2. Copy the code block into your executor.
3. Adjust the variables if needed.
4. Execute and enjoy!

### Discord Invite Opener
```lua
-- Setup Function
loadstring(game:HttpGet("https://raw.githubusercontent.com/SuroxWare/Utils/refs/heads/main/discord"))()

-- Call Function
local result = _G.Open_Discord("Your Invite")

-- Show Result (Optional)
print(result)
```

> **Notes**
> * You can use the full invite link or just the invite code.
> * Some executors can't open Discord, in this case the full invite link will be copied.
> * In case an executor doesn't support `setclipboard` the function will return `Failed`
> * Result will be one of these values: `"Opened"`, `"Copied"`, `"Failed"`
