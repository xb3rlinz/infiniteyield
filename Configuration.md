# Configuration
Set these globals before running the script.
```lua
_G.notification = true   -- default
_G.silentload   = false  -- default
_G.loadinfy     = true   -- default
_G.loadexec     = false  -- default
_G.loaddex      = false  -- default
```
---
## Keys
### `_G.notification`
**Default:** `true`

Shows a notification when scripts are done loading, listing what was loaded (e.g. `"Infy & DarkDex Loaded!"`). Set to `false` to disable.

---
### `_G.silentload`
**Default:** `false`

Suppresses any UI or side effects from the loader.

---
### `_G.loadinfy`
**Default:** `true`

Loads [Infinite Yield](https://github.com/xb3rlinz/infiniteyield)

---
### `_G.loadinfytest` (not recommended)
**Default:** `false`

Loads the test branch of Infinite Yield. Takes priority over `_G.loadinfy` if both are set.

---
### `_G.loadexec`
**Default:** `false`

Loads in-game executor.

---
### `_G.loaddex`
**Default:** `false`

Loads [DarkDex](https://github.com/xb3rlinz/infiniteyieldbackup) — a game explorer and instance viewer.

---
## Example
```lua
_G.notification = true
_G.loadinfy     = true
_G.loaddex      = true

loadstring(game:HttpGet("https://raw.githubusercontent.com/xb3rlinz/infiniteyield/refs/heads/master/loader"))()
```
