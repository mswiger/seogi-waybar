# Seogi Waybar
Custom Waybar module for the [Seogi IME](https://github.com/mswiger/seogi).
Can be used to display the status of Seogi (i.e., Hangul input enabled/disabled) in a custom Waybar module.

## Configuring Waybar
The Seogi Waybar module can be added to Waybar by adding the following to your Waybar configuration:

```
"custom/seogi": {
	"exec": "seogi-waybar",
	"return-type": "json",
	"signal": 8
}
```

The text displayed when Hangul mode is enabled or disabled,
as well as which signal is sent to Waybar when the status changes, can be configured:

```
"custom/seogi": {
	"exec": "seogi-waybar -e 한 -d EN -s 5",
	"return-type": "json",
	"signal": 5
}
```
