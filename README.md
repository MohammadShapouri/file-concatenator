### How to use it:

1.  Place the script in the root folder of your project (the folder containing `dir1`, `dir2`, etc.).
2.  Run the script:
    ```bash
    python merge_files.py
    ```
3.  A file named `content.txt` will appear in the same folder.

### Key Features of this Script:

1.  **Safety:** It automatically ignores standard junk folders like `node_modules`, `.git`, or python cache folders.
2.  **Binary Protection:** It attempts to read files as UTF-8 text. If it encounters a compiled file or an image, it catches the `UnicodeDecodeError` and skips the file instead of crashing.
3.  **Self-Exclusion:** It ensures it does not write `content.txt` into itself.
4.  **Formatting:** It generates the output exactly as you requested:
    ```text
    dir1/file1.py:
    import os...

    dir2/file2.js:
    console.log("hello")...
    ```
