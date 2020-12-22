# Elbo Display Server and Tiling Window Manager

*Inspired by, but legally distinct, from a popular science fiction franchise
currently owned by an incredibly litigious IP Holder*

It's possible this won't include a display server, as Wayland might end up being
capable enough, but I reserve the right to break with Wayland wherever doing so
makes Elbo better.

The existing TWM aren't "fully featured" the way that Explorer.exe, Finder.app,
KDE, or GNOME are. But when thinking about what goes into "fully featured",
it's hard to keep that list in your head. So I wrote it down to amke sure I
don't forget.

## List of "Features"

Things that it does

* Multi-monitor handling
    * Remembers monitors and positioning of monitors that have been seen before
    * Recovery from bad configurations
    * Mixed DPI-support
    * Things won't screw up rendering if you change DPI on a monitor
    * VRR support
* Multi-touch handling
    * touch events always get mapped to the correct display
    * Drag scrolling and zooming works
    * "Natural" scrolling doesn't exist
    * On-screen keyboard
    * Long press resizing gestures
    * Gesture to handle moving windows across monitors
    * Corner, edge, 5-finger pinch gestures
* Sudden disconnects will gracefully wait a few milliseconds before reconfiguring
* Pop-up panel with current key bindings
* Teacher/video recording keyboard event log mode
* Global keyboard hotkeys
    * Media hotkeys
    * backlight hotkeys
* Clipboard done as a plugin
    * Xserver style highlight clipboard built-in
    * More complex clipboard paste types (images, rich text)
    * Pluggable with advanced clipboard functionality doo-dads
        * Some way to keep passwords out of clipboard history
* Password manager integration
    * because it sucks to be able to log into spotify web, but not the spotify app
    * Almost said discord, and then I remembered QR login
* 2FA manager integration
* Drag-n-drop
    * Windows can't rearrange while dragging
    * multitouch different monitor drop targets
* easy access file browser for uploading files with drag/drop targets on websites
    * Stand on space bar in file browser windows for Preview
* icon tray that doesn't suck
    * Also user gets to hide icons, because application writers have no idea what's good experience
* Network up/down, Internet connectivity icon/notification
* istatmenus style expandable menus
    * It's gotta be way way way easier to configure than conky
* Workspaces
    * summonable/banishable windows
    * REALLY GOOD window positioning
        * Line up windows into a brace/rule, and put trees and splits together
    * Composable workspaces so you can have "sticky" splits
* No title bars
* Live window previews
* App drawer
* Support GIMP/macos style programs (lots of little windows)
* Infinite canvas
* Notifications that don't suck for the user
    * User rules for when to see notifications, and when to auto-toss notifications
    * Or just turn off notifications. They're dumb anyway.
* Beep-boop and silent modes
* Bring back Android Holo style. Discourage "material"
* Built in screenshot, screen recording stuff (done as a plugin)
* Good OBS support: capturable desktops, windows, portions of windows, capturable windows even when not actively displayed, etc
* Modals and dialogues float by default
* Need to make sure Android Studio doesn't screw up real hard
* eGPU, Multi-GPU, GPU-passthrough, Optimus support
* A way to set environment variables for the session
* Live-reload
* Force a window repaint
* Config files and config dialogues
* Please don't make me learn XKB
    * Should be able to have neo-style keyboard layouts
* Pop-out floating video mini-player support. Even if you have to lie to windows to make them believe they're fullscreen
* Set split ratios
* Ability to crop windows to fit into small splits
    * Enforce window sizes, aspect ratios
    * Parallax scroll cropping
    * Fixed cropping
    * key combo to stop sending mouse events to window (for parallax scrolling to be fixed)
* Easy way to kill programs. Not minimize to tray
* Multi-language support
* Hot language swap. None of this "You need to log out and log back in to apply changes"
* Quick input language change
* IME support
* alt-code/colon-emoji-colon substitution/global special character panel (macos style)

* OLED helper optional settings
    * pixel shift
    * static elements significantly dimmed
