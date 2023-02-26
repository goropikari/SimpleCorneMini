```bash
QMK_VERSION=0.19.10 ./docker_build.sh corne_mini:default:flash
```

`SPLIT_HAND_PIN` を使っているので PCB 裏面のジャンパーをブリッジさせる必要あり。
ブリッジさせない場合は corne の firmware を素直に焼く

ブリッジさせる面を間違えたときは `#define	SPLIT_HAND_PIN_LOW_IS_LEFT` を入れれば多分大丈夫

https://github.com/qmk/qmk_firmware/blob/0.19.10/docs/feature_split_keyboard.md#handedness-by-pin
