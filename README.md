# Tagged file Concatenation to Clipboard

This is a Python script that allows users to concatenate multiple files into a single copy-paste buffer. This buffer can then be pasted into any text input area, including the chat interface of ChatGPT. This tool is especially useful when you want to provide code context to ChatGPT. 

<img width="341" alt="Screenshot" src="https://github.com/filipe-m-almeida/copy-files/assets/28849172/c10f9113-c697-40ac-8cb4-c376b91596db">

## Requirements

- Python 3
- `pyperclip`
- `urwid`

## Usage

To use the script, run the following command in the terminal:

```bash
gpt-copy-files [file1] [file2] ...
```

You can also use wildcards to select multiple files:
```bash
gpt-copy-files script.py src/*
```

## Key Bindings

The script supports the following key bindings:
| Key       | Description                     |
| --------- | ------------------------------- |
| ? or h    | Show the help screen.           |
| Enter     | Perform an action on selected files. |
| Space     | Toggle selection of current file. |
| c         | Check all files.                |
| s         | Uncheck all files.              |
| t         | Toggle selection of files.      |
| q or esc  | Exit the program.               |

## Functionality

Once the script is run, it presents a checklist of the specified files. Users can select or unselect the files they wish to include in the buffer. After the files are chosen, pressing 'Enter' will concatenate the content of the files, commenting the beginning of each file's content with the filename and the appropriate comment style (# or //, depending on the file's extension), and copy this text to the clipboard. Users can then paste this text wherever they need.

## Contact

For any issues or suggestions, please reach out to the author Filipe Almeida filipe.almeida@gmail.com.
