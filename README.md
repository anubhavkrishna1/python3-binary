# python3-binary

Binary files for Python 3.

## Usage

This repository provides pre-built Python binaries for Linux. Follow the steps below to use them:

1. **Download the Binary**
   - Navigate to the [Releases](https://github.com/ anubhavkrishna1/python3-binary/releases) section of this repository.
   - Download the appropriate binary archive (`.tar.gz` or `.zip`) for your desired Python version and architecture.

2. **Extract the Binary**
   - For `.tar.gz` files:
    ```bash
     tar -xvzf python-<version>-linux-<arch>.tar.gz
     ```
     ```bash
     tar -xvzf python-<version>-linux-<arch>.tar.gz -C /desired/path
     ```
   - For `.zip` files:
    ```bash
     unzip python-<version>-linux-<arch>.zip
     ```
     ```bash
     unzip python-<version>-linux-<arch>.zip -d /desired/path
     ```

3. **Set Up Environment**
   - Add the extracted binary directory to your `PATH`:
     ```bash
     export PATH=/desired/path/bin:$PATH
     ```
   - Verify the installation:
     ```bash
     python3 --version
     ```

4. **Start Using Python**
   - You can now use the custom Python binary for your projects.
