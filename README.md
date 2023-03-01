For original levee look in [here](https://sr.ht/~andreafeletto/levee/)
# levee-tuhkis

levee is a statusbar for the [river] wayland compositor, written in [zig]
without any UI toolkit. It currently provides full support for workspace tags
and displays pulseaudio volume, battery capacity and screen brightness.
<br>
Uses the FiraCode Nerd Font for the icons in the bar.
## Build

```
git clone --recurse-submodules https://github.com/Tuhkis/levee-tuhkis.git
cd levee-tuhkis
zig build
```
Then copy `zig-out/bin/levee` to `/usr/bin/` or somewhere else in the `PATH`.

## Usage

Add the following toward the end of `$XDG_CONFIG_HOME/river/init`:

```
riverctl spawn "levee pulse backlight battery"
```

## Dependencies

* [zig] 0.10.0
* [wayland] 1.21.0
* [pixman] 0.42.0
* [fcft] 3.1.5
* [libpulse] 16.0
* [FiraCode Nerd Font]

## Contributing

Please join the [#levee] IRC channel to ask for help or to give feedback.
You are welcome to send patches to the [mailing list] or report bugs on the
[issue tracker].
If you aren't familiar with `git send-email`, you can use the [web interface]
or learn about it by following this excellent [tutorial].

[river]: https://github.com/riverwm/river/
[zig]: https://ziglang.org/
[wayland]: https://wayland.freedesktop.org/
[pixman]: http://pixman.org/
[fcft]: https://codeberg.org/dnkl/fcft/
[libpulse]: https://www.freedesktop.org/wiki/Software/PulseAudio/
[#levee]: ircs://irc.libera.chat/#levee
[mailing list]: https://lists.sr.ht/~andreafeletto/public-inbox
[issue tracker]: https://todo.sr.ht/~andreafeletto/levee
[web interface]: https://git.sr.ht/~andreafeletto/levee/send-email
[tutorial]: https://git-send-email.io
[FiraCode Nerd Font]: https://www.nerdfonts.com/font-downloads
