# Minecraft World Loader and Downloader (MWL)

Minecraft World Loader (MWL) is a simple console application designed to help Minecraft players easily download and extract world files into their local Minecraft installation. The tool automates the process of selecting the Minecraft folder, extracting world files from a ZIP archive, and launching Minecraft after the process is complete.

## Features

- **Automatic Minecraft Folder Detection**: Automatically detects the Minecraft installation folder or allows users to select it manually.
- **Download and Extract Worlds**: Select a ZIP file containing the Minecraft world, and the application will extract it to the appropriate location.
- **Minecraft Launcher Integration**: After extracting the world, the program can launch Minecraft automatically.
- **Update Check**: The program checks if a newer version of MWL is available and offers to download and install it.
- **Configuration**: The program saves the path of the Minecraft folder for future use in a configuration file (`mwl_config.json`).

## Requirements

- **.NET 6.0 or later**: The application is built with .NET and requires version 6.0 or later.
- **Windows OS**: The program uses Windows Forms components (`FolderBrowserDialog`, `OpenFileDialog`), which are Windows-specific.
- **Minecraft**: A valid Minecraft installation is required.

## How to Use

### 1. **Download the Latest Version**
   Download the latest version of MWL from the [releases page](https://github.com/yourusername/minecraft-world-loader/releases).

### 2. **Run the Application**
   After downloading the executable, run the program by double-clicking it or using the command line.

### 3. **Check for Updates**
   The program will check if a newer version is available. If an update is found, you will be asked if you want to download and install it.

### 4. **Minecraft Folder Selection**
   - The program will attempt to automatically detect your Minecraft folder. If it's not detected, you will be prompted to manually select the folder.
   - Once the folder is selected, it will be saved in the `mwl_config.json` file for future use, so you won’t need to select it again.

### 5. **Select World ZIP File**
   The program will prompt you to select a ZIP file containing the Minecraft world you want to download. It will extract the contents of the ZIP file to the `saves` folder of your Minecraft installation.

### 6. **Enter World Folder Name**
   After selecting the ZIP file, you will be asked to enter the name of the world folder. The program will create a folder with that name in the `saves` directory and extract the world files there.

### 7. **Launch Minecraft**
   After the world is successfully extracted, you will be asked if you want to launch Minecraft. If you choose "Yes", the Minecraft launcher will open automatically.

## Configuration

The application saves the path to your Minecraft folder in a configuration file called `mwl_config.json`. This allows the program to remember your Minecraft folder for future use. You can manually edit or delete the configuration file if you need to reset the Minecraft folder path.

### Configuration File
- **`mwl_config.json`**: This file stores the path of your Minecraft installation folder and other settings.

## Troubleshooting

- **Minecraft Folder Not Detected**:  
  If the program does not automatically detect the Minecraft folder, ensure that Minecraft is installed in the default directory (`C:\Users\<YourUserName>\AppData\Roaming\.minecraft`). If it is located in a custom directory, you can manually select the folder when prompted.

- **Invalid World ZIP File**:  
  Ensure that the ZIP file you select contains the correct folder structure for a Minecraft world (e.g., `level.dat`, `region`, `playerdata`).

- **Application Crashes**:  
  If the program crashes, try running it as an administrator, or check the `mwl_config.json` configuration file for issues.

## Donate

If you find MWL useful and would like to support its development, you can make a donation via the following links:

- **Ko-Fi**: [Donate via Ko-Fi](https://ko-fi.com/sandwichdev)

Your donations help maintain and improve the application.

## Contributing

MWL is an open-source project, and you are welcome to contribute! You can:

- Report bugs
- Suggest new features
- Submit pull requests with bug fixes or improvements

Feel free to open an issue on the GitHub repository if you encounter any problems or have suggestions.

## License

Minecraft World Loader and Downloader is open-source and released under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

Thank you for using Minecraft World Loader and Downloader! If you need help or have any questions, feel free to reach out via GitHub issues.

