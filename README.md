# binmerge

A Python tool to merge multiple game BIN/CUE files into a single unified file, or split a unified file back into individual tracks.

## How to Use

### 1. Automatic Usage (Easiest)
Navigate to the folder where your game is located and run the command without any parameters:
```bash
./binmerge
```
* **Single .cue file in the folder:** Merges automatically.
* **Multiple .cue files in the folder:** Displays a numbered menu for you to choose which one to process.

### 2. Manual Usage
* **Merge tracks:**
  ```bash
  ./binmerge "/path/to/Game.cue" "Game (Merged)"
  ```
* **Set an output folder (`--outdir`):**
  ```bash
  ./binmerge --outdir "/path/to/destination" "/path/to/Game.cue" "Game (Merged)"
  ```
* **Split tracks:**
  ```bash
  ./binmerge --split "/path/to/Game.cue" "Game_Split"
  ```
* **Batch processing (`--batch`):**
  Processes all `.cue` files within a directory sequentially:
  ```bash
  ./binmerge --batch "/path/to/folder"
  ```

## Quick Tips
* **Spaces in paths:** Always wrap the path in double quotes `""` when running commands manually.
* **Terminal help:** Run `./binmerge --help` to view all available options (`--force`, `--verbose`, `--buffer-mb`, etc.).
