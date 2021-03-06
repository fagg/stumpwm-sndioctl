# stumpwm-sndioctl

stumpwm-sndioctl adds some features to StumpWM so you can control the
volume using OpenBSD's sndioctl, and have it show you pretty messages
as you make changes.

Add something like this to your StumpWM config:
```
(ql:quickload :stumpwm-sndioctl)
(define-key *top-map* (kbd "XF86AudioMute") "toggle-mute")
(define-key *top-map* (kbd "XF86AudioLowerVolume") "volume-down")
(define-key *top-map* (kbd "XF86AudioRaiseVolume") "volume-up")
```

The code is documented in Lisp style (i.e. self documenting), see
`stumpwm-sndioctl.lisp` for all the knobs you can turn.

## License

Copyright 2021, Dr Ashton Fagg <ashton@fagg.id.au>

Permission to use, copy, modify, and/or distribute this software for
any purpose with or without fee is hereby granted, provided that the
above copyright notice and this permission notice appear in all
copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL
WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE
AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL
DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR
PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER
TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
PERFORMANCE OF THIS SOFTWARE.


