

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

``` xml
<property name="mode" type="uint" value="0"/>
```

> 1: Vertical

``` xml
<property name="mode" type="uint" value="1"/>
```

> 2: Deskbar

``` xml
<property name="mode" type="uint" value="2"/>
```




## Panel Position



## deskbar-left

> ~/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-panel.xml

``` xml
<property name="mode" type="uint" value="2"/>
<property name="position" type="string" value="p=6;x=0;y=0"/>
```




## deskbar-right

> ~/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-panel.xml

``` xml
<property name="mode" type="uint" value="2"/>
<property name="position" type="string" value="p=2;x=0;y=0"/>
```




## panel-top

> ~/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-panel.xml

``` xml
<property name="mode" type="uint" value="0"/>
<property name="position" type="string" value="p=6;x=0;y=0"/>
```




## panel-bottom

> ~/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-panel.xml

``` xml
<property name="mode" type="uint" value="0"/>
<property name="position" type="string" value="p=8;x=0;y=0"/>
```




## panel-left

> ~/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-panel.xml

``` xml
<property name="mode" type="uint" value="1"/>
<property name="position" type="string" value="p=6;x=0;y=0"/>
```




## panel-right

> ~/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-panel.xml

``` xml
<property name="mode" type="uint" value="1"/>
<property name="position" type="string" value="p=2;x=0;y=0"/>
```



## Notice

``` xml
		<property name="plugin-12" type="string" value="launcher">
			<property name="items" type="array">
				<value type="string" value="featherpad.desktop"/>
			</property>
		</property>
```

> run `xfce4-panel -p` failed, if `featherpad.desktop` not exist in `/usr/share/applications/featherpad.desktop`.
