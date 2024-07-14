---
title: "Installing Hugo on PC"
weight: 1
---

This guide will walk you through the process of installing Hugo on your PC.

## Windows

1. Download the latest Hugo release from the [official Hugo releases page](https://github.com/gohugoio/hugo/releases).
2. Extract the ZIP file to a folder, e.g., `C:\Hugo\bin`.
3. Add the Hugo executable to your PATH:
   - Right-click on 'This PC' and go to 'Properties'.
   - Click on 'Advanced system settings'.
   - Click on 'Environment Variables'.
   - Under 'System variables', find the 'Path' variable, select it and click 'Edit'.
   - Click 'New' and add the path to your Hugo executable (e.g., `C:\Hugo\bin`).
   - Click 'OK' to save your changes.

4. Open a new command prompt and run `hugo version` to verify the installation.

## macOS

1. Install Homebrew if you haven't already: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
2. Run `brew install hugo`
3. Verify the installation by running `hugo version`

## Linux

For most Linux distributions, you can install Hugo using your package manager. For example:

- Ubuntu or Debian: `sudo apt-get install hugo`
- Fedora, Red Hat, or CentOS: `sudo dnf install hugo`

After installation, verify by running `hugo version`.

Now you're ready to start creating your Hugo site!