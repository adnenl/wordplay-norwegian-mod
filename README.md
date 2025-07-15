# Word Play Norwegian Mod

This repository contains a custom Norwegian dictionary and letter bag mod for the game **Word Play** by Game Maker's Toolkit.

---

## About

Word Play is designed primarily for English, with its dictionary and letter bag balanced around English word properties.

This mod enables playing **Word Play** in Norwegian by providing:

- A **custom Norwegian dictionary** based on the official word list from [Norsk Scrabbleforbund](https://www2.scrabbleforbundet.no/?p=4939)
- A **custom letter bag** with tile values and distributions from Norwegian Scrabble rules

> **Note:** This is an experimental and unsupported feature in Word Play. Use at your own risk.

---

## How to Use This Mod

### 1. Find Your Save Game Folder

The custom dictionary and letter bag files must be placed in the same folder as your Word Play save data.

| Platform | Save Folder Path                                   |
|----------|--------------------------------------------------|
| **Mac**  | `/Users/YourUserName/Library/Application Support/com.GMTK.WordPlay` |
| **PC**   | `C:\Users\YourUserName\AppData\LocalLow\Game Maker's Toolkit\Word Play` |

*You may need to show hidden files and folders to access these locations.*

---

### 2. Add the Custom Dictionary

Create a file named `customdictionary.txt` inside the save folder.

- The file should contain every Norwegian word you want the game to accept.
- Use **CAPITAL LETTERS**.
- List words in **alphabetical order**.
- Non-Latin characters (like Æ, Ø, Å) are supported if your system/font supports UTF-8.

---

### 3. Add the Custom Letter Bag

Create a file named `customletterbag.txt` in the same folder.

- Each line should be a 5-character code:
  - 1st character: Letter (e.g., `A`, `Æ`, `Ø`, `Å`)
  - Next two digits: Tile value (e.g., `01` for 1 point)
  - Last two digits: Number of tiles (e.g., `07` for seven tiles)

Example line:

```plaintext
A0107
```

means 7 tiles of the letter A, each worth 1 point.

The Norwegian letter bag values and distributions are based on the official Norwegian Scrabble rules.

---

### Reverting to English

To revert back to the standard English game:

- Delete `customdictionary.txt` and/or `customletterbag.txt` from the save folder.
- Restart Word Play.

---

## Important Notes and Limitations

- This modding method is experimental and unofficial.
- Do not use this on the pre-release demo version.
- Incorrect formatting can break the game.
- Some non-Latin characters might display as squares if your font does not support them.
- This mod only changes accepted words and letter tiles; UI and game text remain English.

---

## Credits

- Word Play by Game Maker's Toolkit
- Norwegian word list sourced from Norsk Scrabbleforbund
- Tile values and distributions based on Norwegian Scrabble rules

---

Good luck, and have fun playing Word Play in Norwegian!

Made by adnenl
Inspired by the official Word Play modding guide by Mark Brown.