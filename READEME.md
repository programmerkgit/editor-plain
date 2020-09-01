##
HTMLElement - token - document: 対応づけ

## Event
- focus
https://developer.mozilla.org/en-US/docs/Web/Events
## Key
- keydown
- keypress
- keyup
## Mouse
- auxclick
- click
- dbclick
- contextmenu
- mousedown
- mouseenter
- mouseleave
- mousemove
- mouseover
- mouseout
- mouseup
- pointerlockchange
- pointerlockerror
- select
- wheel
## Drag
- drag
- dragend
- dragenter
- dragstart
- dragleave
- dragover
- drop

## Notion
mouse moveで選択エリアを作っている。
選択エリアの一に応じて選択範囲を決定している。
keydownでctrl + Aを検知している。
titleでkeydownしたらデフォルトのイベントをキャンセルして要素を作るようになっている。

- 要件を詳細に洗い出す
