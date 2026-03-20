# Configuration
Place these globals above the loader.
```lua
_G.notification = true   -- default
_G.silentload   = false  -- default
_G.loadinfy     = true   -- default
_G.loadexec     = false  -- default
_G.loaddex      = false  -- default
```
---
## Keys
### `_G.loadinfytest` (not recommended)
**Default:** `false`

Loads the test branch of Infinite Yield. Takes priority over `_G.loadinfy` if both are set.

---
### `_G.notification`
**Default:** `true`

Shows a notification when scripts are done loading, listing what was loaded (e.g. `"Infy & DarkDex Loaded!"`). Set to `false` to disable.

---
### `_G.silentload`
**Default:** `false`

Automatically hides IY when executed.

---
### `_G.loadinfy`
**Default:** `true`

Loads [Infinite Yield](https://github.com/xb3rlinz/infiniteyield)

---
### `_G.loadexec`
**Default:** `false`

Loads in-game [executor](https://github.com/xb3rlinz/infiniteyieldbackup/blob/main/executor.lua)

---
### `_G.loaddex`
**Default:** `false`

Loads [DarkDex](https://github.com/LorekeeperZinnia/Dex)

---
## Example
```lua
_G.notification = true
_G.silentload   = true
_G.loaddex      = true

loadstring(game:HttpGet("https://raw.githubusercontent.com/xb3rlinz/infiniteyield/refs/heads/master/loader"))()
```
