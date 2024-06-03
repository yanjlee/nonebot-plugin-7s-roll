### Roll Dice Plugin

Roll Dice is a small utility for dice rolling, compatible with NoneBot2 2.0 API and supports OneBot V11.

#### Usage:
```python
nonebot.load_plugin("nonebot_plugin_7s_roll")
nonebot.run()
```
`.env` file configuration:
```env
I7S_ROLL_COMMAND="roll"
I7S_ROLL_TRIGGER="roll"
```

#### Command:
```plaintext
roll [[ ][ ]] 
```
- `roll` format: `[d|D][ ][ ]`
  - `<count>`: Number of rolls (up to 20)
  - `<sides>`: Number of sides (up to 1000)
  - `<method>`: `sum`, `min`, `max`, `avg`

#### Examples:
- `roll 3d6`: 
  ```text
  3d6 投掷结果
  第 1 颗：5
  第 2 颗：5
  第 3 颗：6
  总和为 16
  ```
- `roll 3d10+2d6+1 >20`:
  ```text
  3d10+2d6+1 投掷结果(目标 > 20)：(5 + 1 + 9) + (4 + 5) + 1 = 25，通过
  ```
- `roll 3d100max+4d10`:
  ```text
  3d100max+4d10 投掷结果 (max[35, 60, 29] = 60) + (1 + 1 + 5 + 8) = 75
  ```

#### Screenshot:
![screenshot-dice](https://rikka.7sdre.am/files/8c6c5b15-0343-4d14-a203-422c7d6c634e.png)

#### LICENSE:
MIT

[Original Markdown file](https://raw.githubusercontent.com/yanjlee/nonebot-plugin-7s-roll/main/README.md).
