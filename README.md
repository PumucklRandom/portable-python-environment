# Portable Python Environment

## Overview

The `create_portable_env.py` script creates a portable Python environment for Windows by downloading and configuring an embeddable Python distribution.

## What it does

- Downloads the embeddable Python version matching the current activated Python environment
- Installs pip in the portable environment
- Installs all dependencies from the current activated Python environment via `pip freeze`
- Optionally cleans up unnecessary files to reduce size (packages, pychache, Scripts, files/folders, *.dist-info, pip)

## Use cases

- Create standalone Python applications that don't require an avaiable Python environment
- Package your scripts/project/app with its own isolated Python environment
- Distribute applications without dependency conflicts

## Note

**This portable Python environment is only usable for Windows.**

The script uses Windows-specific embeddable Python distributions (.exe files) and is designed for Windows architecture (win32/amd64).
