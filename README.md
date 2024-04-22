![shell helper mascot](./asset/shellhelper.jpg)

# Shell Helper

This repository is a collection of useful bash scripts for several common file and directory manipulation tasks on the Linux/Unix system. Each script is designed to facilitate specific operations, such as checking for the existence of a path, creating files or directories, editing files, or exploring directories.

## Available Stripts

Following are the scripts available in this repository:

- **exists:** Checks whether a path (file or directory) exists on the file system.
- **new:** Creates a new file at the specified path, creating the necessary directories if they do not exist.
- **edit:** Opens a file for editing using the editor configured in the `EDITOR` environment variable.
- **explore:** Opens a directory for exploration using the file manager configured in the `FILEMANAGER` environment variable.
- **open:** Opens a file or directory for editing or exploration based on the existence and type of the specified path.

## Setup

Clone this repository in your home directory.

```sh
git clone https://github.com/ortense/shellhelper.git ~/.shellhelper
```

Setting the EDITOR and FILEMANAGER environment variables as needed for the edit and explore scripts, respectively.


For example, if you use [vim](https://github.com/vim/vim) and [ranger](https://github.com/ranger/ranger), ensure the environment variables are configured as follows:

```sh
export EDITOR=vim
export FILEMANAGER=rider
export SHELLHELPER="$HOME/.shellhelper/bin"
export PATH="$PATH:$SHELLHELPER"
```

Give execute permission to all files in the bin folder:

```sh
chmod +x ~/.shellhelper/bin/*
```

## License

This repository is licensed under the MIT License. See the LICENSE file for details.
