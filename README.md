# LXDE Fix panel strut script

lxfixstrut is a simple bash script to fix LXDE panel showing over windows.

This script uses `xwininfo` to find the panel window id, and uses `xprop` to set the correct `_NET_WM_STRUT_PARTIAL`.

## Usage:
`lxfixstrut $DISPLAY_RESOLUTION_X $PANEL_HEIGHT`

For example you can put the following command in .bashrc to fix the panel spacing at startup:
`lxfixstrut 1366 32`
