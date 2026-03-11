# cmdlinemader

A command-line tool that converts shell scripts (`.sh` files) into binary executables using [SHC (Shell Script Compiler)](https://github.com/neurobin/shc). The resulting binary is automatically moved to your system's PATH so it can be run as a regular command.

> **Note:** This project is still under active development.

## Features

- Converts `.sh` shell scripts into compiled binary executables
- Prompts for a custom name for the output binary
- Automatically installs the binary to `/usr/sbin` for system-wide access
- Cleans up intermediate build files

## Prerequisites

Make sure your system packages are up to date and that `shc` is installed:

```bash
sudo apt update -y && sudo apt upgrade -y
sudo apt install shc
```

## Installation

```bash
git clone https://github.com/anonymousc/cmdlinemader.git
cd cmdlinemader
chmod +x cmder
```

## Usage

Run the tool with:

```bash
sudo ./cmder
```

You will be prompted to:

1. Enter the path to your `.sh` script
2. Choose a name for the output binary

The tool will compile your script and place the resulting binary in `/usr/sbin`, making it available as a system command.
