# FYProject
1.	Download Visual Studio Community Edition:
o	Go to the official Visual Studio download page: https://visualstudio.microsoft.com/downloads/
o	Download the Community edition (it's free for individual developers).
2.	Run the Visual Studio Installer:
o	Double-click the downloaded installer.
o	When the installer opens, you'll see a list of "Workloads." This is the crucial step.
o	Select the "Desktop development with C++" workload. Make sure the checkbox next to it is ticked.
o	On the right-hand side, under "Installation details", you might want to specifically check for MSVC v143 - VS 2022 C++ x64/x86 build tools (or MSVC v142 - VS 2019 C++ x64/x86 build tools if you choose an older VS version, but 2022 is fine).
o	Click "Install" and let it complete. This might take a while, as it's a large download.
3.	Reboot Your Computer: After Visual Studio and the C++ build tools are installed, reboot your computer. This ensures that all necessary environment variables and paths for the compilers are correctly set.
1. Install CMake 🛠️
CMake is a cross-platform build system generator that dlib uses to compile its C++ parts.
1.	Download CMake:
o	Go to the official CMake website: https://cmake.org/download/
o	Look for the Windows x64 Installer (.msi) (e.g., cmake-3.XX.X-windows-x86_64.msi). Download the latest stable version.
2.	Run the CMake Installer:
o	Double-click the downloaded .msi file to start the installation.
o	Crucially, during the installation process, ensure you select the option to "Add CMake to the system PATH for all users" or "Add CMake to the system PATH for the current user." This is vital so that your command prompt can find the cmake executable.
3.	Reboot Your Computer: After installing CMake and adding it to the PATH, reboot your computer for the changes to take effect system-wide.








1. Install Visual C++ Redistributable Packages 📦
dlib's Python bindings are compiled with C++ compilers, and they depend on runtime libraries provided by Microsoft Visual C++. Even if you have Visual Studio installed, you might need these specific redistributable packages.
•	Download and install the latest "Visual C++ Redistributable for Visual Studio 2015, 2017, 2019, and 2022":
1.	Go to the official Microsoft download page: https://learn.microsoft.com/en-us/cpp/windows/latest-supported-visual-c-plus-plus-redistributable-downloads
2.	Under "Visual Studio 2015, 2017, 2019, and 2022", download both vc_redist.x64.exe (for 64-bit systems, which is most common) and vc_redist.x86.exe (for 32-bit compatibility, sometimes needed).
•	Reboot your computer after installing/repairing these redistributables. This is crucial for system paths to update.
On VS CODE:
pip install opencv-python Pillow
pip install dlib
pip install face-recognition
