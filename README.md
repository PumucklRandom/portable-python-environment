# Portable Python Environment

## Overview

This script creates a portable Python environment for Windows by downloading and configuring an embeddable Python distribution.

## What it does

- Downloads the embeddable Python version matching your current Python installation
- Installs pip in the portable environment
- Copies all dependencies from your current Python environment
- Optionally cleans up unnecessary files to reduce size (cache, dist-info, etc.)

## Use cases

- Create standalone Python applications that don't require system-wide Python installation
- Package your project with its own isolated Python environment
- Distribute applications without dependency conflicts

## Note

**This portable Python environment is only usable for Windows.**

The script uses Windows-specific embeddable Python distributions (`.exe` files) and is designed for Windows architecture (win32/amd64).
