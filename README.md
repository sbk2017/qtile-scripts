# Qtile scripts

## qtilekey

List all binding keys from qtile config file.
required :
``` bash
pip install rich
pip install click
```
## Usage:

``` bash
qtilekeys --help
Usage: qtilekeys [OPTIONS]

Options:
  --keys         Sort by keys [default]
  --config       Sort as config file
  --search TEXT  Search for word in description
  --help         Show this message and exit.

```
The default sorting is by keys alphabet. 
``` --config ``` will sort the keys list as it is in config file.
``` --search ``` will only give result of keys that include the search word.
### Example:
``` bash
qtilekeys --search layout
┏━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━┓
┃ Modifier ┃ Key    ┃ Desc                   ┃
┡━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━┩
│ mod4     │ Tab    │ Toggle between layouts │
│ mod4     │ z => g │ Layout grow            │
│ mod4     │ z => m │ Layout maximize        │
│ mod4     │ z => n │ Layout normalize       │
│ mod4     │ z => s │ Layout shrink          │
└──────────┴────────┴────────────────────────┘

qtilekeys --search firefox
┏━━━━━━━━━━┳━━━━━┳━━━━━━━━━━━━━━━━┓
┃ Modifier ┃ Key ┃ Desc           ┃
┡━━━━━━━━━━╇━━━━━╇━━━━━━━━━━━━━━━━┩
│ mod4     │ f   │ Launch firefox │
└──────────┴─────┴────────────────┘

qtilekeys --config --search window
┏━━━━━━━━━━━━━━┳━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃ Modifier     ┃ Key   ┃ Desc                                       ┃
┡━━━━━━━━━━━━━━╇━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
│ mod4         │ space │ Move window focus to other window          │
│ mod4 + shift │ Left  │ Move window to the left                    │
│ mod4 + shift │ Right │ Move window to the right                   │
│ mod4 + shift │ Down  │ Move window down                           │
│ mod4 + shift │ Up    │ Move window up                             │
│ mod4 + mod1  │ Left  │ Grow window down                           │
│ mod4 + mod1  │ Right │ Grow window up                             │
│ mod4         │ m     │ Maximize active window size                │
│ mod4         │ n     │ Reset all window sizes                     │
│ mod4         │ w     │ Kill focused window                        │
│ mod4 + shift │ 1     │ Switch to & move focused window to group 1 │
│ mod4 + shift │ 2     │ Switch to & move focused window to group 2 │
│ mod4 + shift │ 3     │ Switch to & move focused window to group 3 │
│ mod4 + shift │ 4     │ Switch to & move focused window to group 4 │
│ mod4 + shift │ 5     │ Switch to & move focused window to group 5 │
│ mod4 + shift │ 6     │ Switch to & move focused window to group 6 │
│ mod4 + shift │ 7     │ Switch to & move focused window to group 7 │
│ mod4 + shift │ 8     │ Switch to & move focused window to group 8 │
│ mod4 + shift │ 9     │ Switch to & move focused window to group 9 │
└──────────────┴───────┴────────────────────────────────────────────┘
```

# Screenshot:

![screenshot](/2022-08-19-172722_616x1043_scrot.png)
