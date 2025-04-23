Update config.h

- unzip the firmware and run commands in it
- or use `qmk setup` check the official docs
- set `#define SPLIT_USB_DETECT` to enable proper usb detection
- TRS wiring both halves the same PIN 3 for data, vcc and gnd
- flash with qmk software
- build with `qmk compile -kb handwired/dactyl_manuform/5x6 -km default`
- flash with `qmk flash -kb handwired/dactyl_manuform/5x6 -km default` - if want cli
- if needed to convert keymap.json to keymap.c use `qmk json2c -i keymap.json -o keymap.c` and put it in `keymaps/default/` for desired keyboard
