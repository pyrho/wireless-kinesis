# Building
- Do your edits
- cd to your zmk/app directory
- enable the virtual env
    - `$> source ~/code/random/zephyrproject/.venv/bin/activate`
- run `$> west build --pristine -b nice_nano_v2 -- -DSHIELD=wireless_kinesis -DZMK_EXTRA_MODULES=/Users/pyrho/code/personal/wireless-kinesis`
- plug in the keyboard and put it in bootloader mode
    - if you don't have a bind for this, resetting the keyboard 3 times quickly should
      put it in bootloader mode
- run `$> cp build/zephyr/zmk.uf2 /Volumes/NICENANO/.`
