# How to add a Application

This guide explains how to use the script to add new applications

1. **Open PowerShell 7**:

   - Typing the following command:

   ```Powershell title="Powershell 7"
     .\newApp.ps1
   ```

## **Choose the Download Method**:

- You will be presented with two options for the download method:
  1.  **API [Choco/Winget] Recommended**: Use Chocolatey or Winget to download the application.
  2.  **Default [HttpClient] Custom**: Use HttpClient to download the application from a custom URL.
- Select the appropriate method by entering the corresponding number.

## **Enter Application Details**:

- **Application Name**: Enter the name of the application.
- **Application Description**: Enter a description for the application.
- **Download Details**:
  - If you selected **API [Choco/Winget] Recommended**:
    - Enter the **Chocolatey package name** (e.g., `choco install <package>`).
    - Enter the **Winget package ID** (e.g., `winget install -e --id <package>`).
  - If you selected **Default [HttpClient] Custom**:
    - Enter the **file URL** (e.g., `https://example.com/setup.exe`).
    - Enter the **launcher name** (e.g., `setup.exe`).
    - Choose whether the file is **portable** or an **installer**.
    - Enter any **arguments** for the installer (e.g., `/silent`).

## **Select the Application Category**:

- You will be prompted to choose a category for the application from a predefined list (e.g., Web Browsers, Media, Utilities, etc.).
- Select the appropriate category by entering the corresponding number.

  - The script will automatically append the new application details to the `Applications.json` file.

## Build and run

### Test your changes and make Pull Request.
