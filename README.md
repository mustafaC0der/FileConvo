# FileConvo

File conversion tools in Lua. These were made as practice to improve my skills in Lua.

> **⚠️ WARNING:** This is in active development. Some features may not work as intended.

## Functionality

- Convert a PNG to JPEG, WebP, and BMP
- Convert a .txt file to PDF, JSON, and CSV
- Convert an audio file (e.g., MP3) to other formats (e.g., WAV)

## Requirements

To use this tool, you need the following dependencies:

- [Lua](https://www.lua.org/)
- [LuaMagick](https://github.com/leafo/magick)
- [DKJSON](https://github.com/LuaDist/dkjson)
- [FFmpeg](https://ffmpeg.org/) (for audio conversion)
- A PDF library for Lua (e.g., [LuaPDF](https://github.com/sensepost/luapdf))

## Installation

1. Install Lua on your system.
2. Install dependencies using LuaRocks:
   ```sh
   luarocks install magick
   luarocks install dkjson
   luarocks install ffmpeg
   ```
3. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/FileConvo.git
   cd FileConvo
   ```

## Usage

Run the script with:

```sh
lua main.lua
```

## Example

Here are some examples of how you can use the tool:

```lua
local image_converter = require("src.convert_image")
local text_converter = require("src.convert_text")
local audio_converter = require("src.convert_audio")

image_converter.convert_image("example.png", "jpg")
text_converter.txt_to_json("example.txt", "example.json")
text_converter.txt_to_csv("example.txt", "example.csv")
text_converter.txt_to_pdf("example.txt", "example.pdf")
audio_converter.convert_audio("example.mp3", "wav")
```

## Contributions

Feel free to contribute by submitting issues or pull requests.

## License

This project is licensed under the MIT License.

---
Designed and developed by Mustafa.
