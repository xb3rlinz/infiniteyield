# Configuration

Set these globals **before** running the script to control its behavior.

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

Whether to show a notification when scripts finish loading. The notification lists every module that was loaded (e.g. `"Infy & DarkDex Loaded!"`).

Set to `false` to suppress all load notifications.

---

### `_G.silentload`

Loads scripts silently without triggering any extra UI or side effects from the loader itself.

---

### `_G.loadinfy`

Loads [Infinite Yield](https://github.com/xb3rlinz/infiniteyield) — a feature-rich admin command script.

> Set `_G.loadinfytest = true` instead to load the experimental test branch.

---

### `_G.loadinfytest`

Loads the test/development branch of Infinite Yield instead of the stable release. Takes priority over `_G.loadinfy` if both are set.

---

### `_G.loadexec`

Loads the executor module from the backup repository.

---

### `_G.loaddex`

Loads [DarkDex](https://github.com/xb3rlinz/infiniteyieldbackup) — a game explorer and instance viewer.

---

## Example

Load DarkDex and Infinite Yield together with notifications enabled:

```lua
_G.notification = true
_G.loadinfy     = true
_G.loaddex      = true
```
