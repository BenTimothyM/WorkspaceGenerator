
# 🚀 Workspace Launcher Generator

![Batch Script](https://img.shields.io/badge/Batch_Script-4D4D4D?style=for-the-badge&logo=windows&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge) 

**Workspace Generator** is a native Windows Batch script (`.bat`) wizard designed to build custom, automated "workspace launcher" scripts. 

> **🌱 Learning Repository:**
> This repository serves as a **learning playground** for advanced Windows batch scripting. The code demonstrates how to use a script to dynamically generate *another* script file (`echo`ing commands into a new `.bat` file), handle interactive user inputs via a command-line wizard, and request automatic UAC privilege elevation. It's a great example of "script-writing-scripts"!

## 📖 Project Description

Opening the exact same websites, tools, and project folders every morning before you start coding or working can be tedious. 

**WorkspaceGenerator** acts as a guided setup wizard. By answering a few simple prompts (like entering your frequently visited URLs and your project directory path), the script will automatically compile and save a personalized `.bat` launcher file for you. Once generated, you can simply double-click that new launcher, and your entire digital workspace will open instantly!

## ✨ Key Features

- 🧙‍♂️ **Interactive CLI Wizard:** An easy-to-follow command-line interface that guides you step-by-step to build your launcher.
- 🌐 **Multi-URL Support:** Configure up to 3 default websites to launch simultaneously in your default browser.
- 📁 **Directory Launching:** Automatically opens your specific project or working directory in Windows Explorer.
- ⚙️ **Dynamic File Generation:** Dynamically writes and creates a new, standalone `.bat` file based entirely on your inputs.
- 🛡️ **Auto-Elevation:** Automatically detects and requests Administrator privileges via UAC to ensure smooth execution and file creation.
- 🚀 **Instant Testing:** Built-in option to immediately launch and test your generated workspace script as soon as it's compiled.

## 💻 Tech Stack

- **Language:** Windows Batch Scripting (`.bat` / `.cmd`)
- **Environment:** Native Windows Command Prompt (CMD)

## 🚀 Installation

Since this is a native batch script, the setup is incredibly simple:

1. **Clone the Repository**
   Open your terminal/CMD and run:
   ```git clone https://github.com/BenTimothyM/WorkspaceGenerator.git```

2. **Run the Script**
Navigate to the cloned folder and locate the `WorkspaceGenerator.bat` file.

## 💡 How to Use

> ⚠️ **IMPORTANT: Administrator Privileges Required**
> This script requires elevated permissions to create new files in protected directories. The script is designed to automatically prompt for these permissions if you don't run it as admin initially.

You can execute the script in two ways:

**Method 1: GUI (Recommended)**

1. Navigate to the folder where you placed `WorkspaceGenerator.bat`.
2. Double-click the file.
3. Click **"Yes"** on the User Account Control (UAC) prompt if it asks for elevated privileges.
4. Follow the on-screen prompts to input your file name, URLs, and directory path.

**Method 2: Command Line**

1. Open the Start Menu, type `cmd`.
2. Click **"Run as administrator"**.
3. Navigate to your target folder using the `cd` command.
4. Run the script:
```WorkspaceGenerator.bat```



**Terminal Output Example:**

```text
===============================================================================
                      DAILY WORKSPACE LAUNCHER GENERATOR                      
===============================================================================
Created by: Ben Timothy | GitHub: [https://github.com/BenTimothyM](https://github.com/BenTimothyM)
===============================================================================

Enter launcher name (Default: MyWorkspace): DevEnvironment

Please enter up to 3 website URLs to open automatically.
(Leave blank and press Enter to skip any URL)
Enter Website URL 1: [https://github.com](https://github.com)
Enter Website URL 2: [https://stackoverflow.com](https://stackoverflow.com)
Enter Website URL 3: 

Please enter the full local path for your project or working directory.
(Leave blank and press Enter to skip)
Enter Project Folder Path: C:\Users\Ben\Projects\MyCode

Generating your workspace script...

===============================================================================
                      SUCCESS! WORKSPACE GENERATED
===============================================================================

Your custom automated launcher has been successfully compiled.

File Location: C:\Users\Ben\Downloads\DevEnvironment.bat

What would you like to do next?
[1] Launch and Test the New Workspace Immediately
[2] Exit

Select an option (1 or 2): 

```

## 🤝 Contributing (Let's Learn Together!)

As this is a dedicated learning repository, contributions are highly encouraged! If you want to add new features or expand the wizard's capabilities, feel free to pitch in. Some ideas include:

* Adding support to launch specific `.exe` applications (like VS Code or Spotify).
* Adding timeout delays between launching URLs so the browser doesn't freeze.
* Assigning a custom icon to the generated launcher.

1. Fork this repository.
2. Create your feature branch (`git checkout -b feature-app-launching`).
3. Commit your changes (`git commit -m 'Add support to launch .exe applications'`).
4. Push to your branch (`git push origin feature-app-launching`).
5. Open a Pull Request.

## 👨‍💻 Credits

This project is developed and maintained by:

* **Ben Timothy** - [@BenTimothyM](https://github.com/BenTimothyM)

## 📜 License

This project is distributed under the **MIT License**. See the `LICENSE` file for more details.
