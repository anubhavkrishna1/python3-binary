# 🐍 python3-binary

Binary files for Python 3.

![GitHub all releases](https://img.shields.io/github/downloads/anubhavkrishna1/python3-binary/total)

## 📦 Available Python Binaries

| Python Version | Platform | glibc | Release Date | Download |
|----------------|----------|-------|--------------|----------|
| 3.12.10 | Linux x86_64 | - | 2025-04-16 | [tar.gz](https://github.com/anubhavkrishna1/python3-binary/releases/download/python-3.12.10-linux/python-3.12.10-linux-x86_64.tar.gz) \| [zip](https://github.com/anubhavkrishna1/python3-binary/releases/download/python-3.12.10-linux/python-3.12.10-linux-x86_64.zip) |
| 3.11.12 | Linux x86_64 | - | 2025-04-21 | [tar.gz](https://github.com/anubhavkrishna1/python3-binary/releases/download/python-3.11.12-linux/python-3.11.12-linux-x86_64.tar.gz) \| [zip](https://github.com/anubhavkrishna1/python3-binary/releases/download/python-3.11.12-linux/python-3.11.12-linux-x86_64.zip) |
| 3.9.22 | Linux x86_64 | 2.36+ | 2025-07-01 | [tar.gz](https://github.com/anubhavkrishna1/python3-binary/releases/download/python-3.9.22-linux-glibc236/python-3.9.22-linux-glibc236-x86_64.tar.gz) \| [zip](https://github.com/anubhavkrishna1/python3-binary/releases/download/python-3.9.22-linux-glibc236/python-3.9.22-linux-glibc236-x86_64.zip) |
| 3.8.20 | Linux x86_64 | - | 2025-04-27 | [tar.gz](https://github.com/anubhavkrishna1/python3-binary/releases/download/python-3.8.20-linux/python-3.8.20-linux-x86_64.tar.gz) \| [zip](https://github.com/anubhavkrishna1/python3-binary/releases/download/python-3.8.20-linux/python-3.8.20-linux-x86_64.zip) |

> 💡 For detailed release notes and checksums, visit the [Releases](https://github.com/anubhavkrishna1/python3-binary/releases) page.

## 🚀 Usage

This repository provides pre-built Python binaries for Linux. Follow the steps below to use them:

1. **📥 Download the Binary**
   
- Navigate to the [Releases](https://github.com/anubhavkrishna1/python3-binary/releases) section of this repository.
- Download the appropriate binary archive (`.tar.gz` or `.zip`) for your desired Python version and architecture.

2. **📦 Extract the Binary**
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

3. **🔧 Set Up Environment**
   
- Add the extracted binary directory to your `PATH`:
  
     ```bash
     export PATH=/desired/path/bin:$PATH
     ```
- Verify the installation:
     
     ```bash
     python3 --version
     ```

4. **💻 Start Using Python**
- You can now use the custom Python binary for your projects.

## 🛠️ Building Your Own Custom Python Version

This repository provides a GitHub Actions workflow to build a custom Python version. Follow the steps below to build your own version:

1. **🍴 Fork the Repository**
   - Click the "Fork" button at the top-right corner of this repository to create your own copy.

2. **👉 Navigate to Actions**
   - Go to the "Actions" tab in your forked repository.

3. **▶️ Trigger the Workflow**
   - Select the "Build and Release Python Binary" workflow from the list.
   - Click the "Run workflow" button.
   - Provide the desired Python version (e.g., `3.11.7`) in the input field.
   - Click "Run workflow" to start the build process.

4. **⏳ Wait for the Build to Complete**
   - The workflow will compile the specified Python version with optimizations and create binary archives.

5. **📤 Download the Artifacts**
   - Once the workflow completes, navigate to the "Actions" tab.
   - Select the completed workflow run.
   - Download the generated binary files from the "Artifacts" section.

6. **✨ Use the Binary**
   - Follow the instructions in the "Usage" section above to extract and use the custom Python binary.
