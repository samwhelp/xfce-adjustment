

# Xfce Panel


## Help

> man xfce4-panel

run

``` sh
xfce4-panel --help
```

show

```
Usage:
  xfce4-panel [OPTION…] [ARGUMENTS...]

Help Options:
  -h, --help                         Show help options
  --help-all                         Show all help options
  --help-gtk                         Show GTK+ Options
  --help-sm-client                   Show session management options

Application Options:
  -p, --preferences=PANEL-NUMBER     Show the 'Panel Preferences' dialog
  -a, --add-items=PANEL-NUMBER       Show the 'Add New Items' dialog
  -s, --save                         Save the panel configuration
  --add=PLUGIN-NAME                  Add a new plugin to the panel
  -r, --restart                      Restart the running panel instance
  -q, --quit                         Quit the running panel instance
  -d, --disable-wm-check             Do not wait for a window manager on startup
  -V, --version                      Print version information and exit
  --display=DISPLAY                  X display to use

```




## Panel Preferences Dialog

run to show `Panel Preferences Dialog`

``` sh
xfce4-panel -p
```

or run

``` sh
xfce4-panel --preferences=0
```




## Panel Mode

> 0: Horizontal

``` sh
<property name="mode" type="uint" value="0"/>
```

> 1: Vertical

``` sh
<property name="mode" type="uint" value="1"/>
```

> 2: Deskbar

``` sh
<property name="mode" type="uint" value="2"/>
```
