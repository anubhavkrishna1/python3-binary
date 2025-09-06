# 🐍 python3-binary

Binary files for Python 3.

![GitHub all releases](https://img.shields.io/github/downloads/anubhavkrishna1/python3-binary/total)

## 🚀 Usage

This repository provides pre-built Python binaries for Linux. Follow the steps below to use them:

1. **📥 Download the Binary**
   
- Navigate to the [Releases](https://github.com/anubhavkrishna1/python3-binary/releases) section of this repository.
- Download the appropriate binary archive for your desired Python version and architecture:
  - `.tar.gz` or `.zip` files for manual extraction
  - `.deb` files for Debian/Ubuntu systems

2. **📦 Install the Binary**

**For Debian/Ubuntu systems (recommended):**
```bash
# Download the .deb file and install
sudo dpkg -i python-<version>-linux-<arch>.deb

# Python will be installed to /opt/python-<version>/bin/
# You can use it directly:
/opt/python-<version>/bin/python3 --version
/opt/python-<version>/bin/pip3 --version

# Or add to your PATH for convenience:
export PATH="/opt/python-<version>/bin:$PATH"
python3 --version
```

**For manual installation:**
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

3. **🔧 Set Up Environment (Manual Installation Only)**
   
- Add the extracted binary directory to your `PATH`:
  
     ```bash
     export PATH=/desired/path/bin:$PATH
     ```
- Verify the installation:
     
     ```bash
     python3 --version
     ```

4. **💻 Start Using Python**
- **Debian/Ubuntu users**: Python is installed to `/opt/python-<version>/` and can be used directly or added to PATH
- **Manual installation users**: You can now use the custom Python binary for your projects.

## 🗑️ Uninstalling (Debian/Ubuntu)

To remove a Python version installed via deb package:

```bash
# List installed custom Python packages
dpkg -l | grep python.*custom

# Remove the package (replace with your specific version)
sudo dpkg -r python3.11-custom

# For glibc236 versions
sudo dpkg -r python3.11-custom-glibc236
```

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
