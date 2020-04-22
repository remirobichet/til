---
title: Gnom Alt-Tab
date: 2020-04-22T12:47:00.406Z
thumbnail: /static/img/gnome-alt-tab.png
summary: Prevent Gnome shell Alt-Tab from grouping windows from similar apps.
tags:
  - linux
---
Ressources: 

* https://superuser.com/a/860001

> * Open `dconf-editor`
> * Go to `org/gnome/desktop/wm/keybindings`
> * Move the value `'<Alt>Tab'` from `switch-applications` to `switch-windows`
> * Optionally move `'<Shift><Alt>Tab'` from `switch-applications-backward `to`switch-windows-backward`
> * If you want `switch-windows` to work across desktops, not just in the current desktop, you can also uncheck `org/gnome/shell/window-switcher/current-workspace-only `(Courtesy of @CharlBotha)
> * Close `dconf-editor`
> * If using X11, press `<Alt>F2`, then type `r `to restart Gnome.

![Gnome Alt-Tab](/static/img/gnome-alt-tab.png "Gnome Alt-Tab")