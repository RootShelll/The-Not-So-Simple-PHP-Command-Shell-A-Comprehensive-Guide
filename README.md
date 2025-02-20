Here’s the complete README.md content formatted for GitHub:

# The Not-So-Simple PHP Command Shell

![PHP Command Shell](images/php-command-shell.png)

## Description

The Not-So-Simple PHP Command Shell is a versatile tool designed for penetration testing and ethical hacking. It helps security professionals enumerate targets and extract information efficiently. This repository provides the necessary files and instructions to set up and use the command shell effectively.

## Features

- **Command Execution**: Execute simple system commands directly from the web interface.
- **File Management**: Upload and download files to and from the target system.
- **User Information Retrieval**: Obtain user permissions and information with a single click.
- **System Information Access**: Quickly access system details and running processes.
- **File Cleanup**: Easily remove all files uploaded through the tool.

## Installation

### Prerequisites

Before using The Not-So-Simple PHP Command Shell, ensure you have the following:

- A web server capable of running PHP.
- Basic knowledge of networking and command-line operations.

### Step-by-Step Guide

1. **Download the Tool**: Clone or download the repository from GitHub.

   ```bash
   git clone https://github.com/kaotickj/The-Not-So-Simple-PHP-Command-Shell.git


Configure the Tool: Open the nsscmdshell.php file and modify the following variables to match your attack machine's IP address and port:

$attackip = "10.0.2.6"; // Replace with your IP
$attackport = "8000";   // Replace with your port


Upload the Shell: Transfer the nsscmdshell.php file to the target server. This step should be performed in accordance with legal and ethical standards.

Access the Shell: Open a web browser and navigate to the uploaded nsscmdshell.php file. You will see a command input interface.

Execute Commands: Type valid commands in the input field or use the provided buttons to execute predefined commands.

Example Command Usage

To run a PowerShell script and save the output:

powershell.exe -ExecutionPolicy Bypass -File .\jaws-enum.ps1 -OutputFilename jaws.txt


After execution, you can download the output file for analysis.

Common Issues and Troubleshooting

If you encounter errors such as:

Warning: file_get_contents(http://XX.XX.XX.XX:XXXX/filename.ext): failed to open stream: No connection could be made...


Consider the following solutions:

Check IP and Port: Ensure that the $attackip and $attackport variables are set correctly.

File Availability: Make sure the files you want to upload are accessible on the specified server and port. You can start a simple HTTP server using:

python3 -m http.server 8000

Ethical Considerations

It is crucial to emphasize that the use of The Not-So-Simple PHP Command Shell should be conducted within the bounds of the law. Unauthorized access to systems is illegal and unethical. Always ensure you have explicit permission to test the target systems.

Learning Resources

For those looking to enhance their skills in ethical hacking, consider exploring the following platforms:

Cybrary
Hack The Box
OWASP
Conclusion

The Not-So-Simple PHP Command Shell is a powerful tool for cybersecurity professionals, enabling efficient target identification and information gathering. By following the guidelines outlined in this document, users can effectively utilize this tool while adhering to ethical standards in cybersecurity.

License

This tool is released under the GPL-2.0 License, allowing modification and redistribution under the same terms.


### Notes:
- Ensure to replace the image paths (e.g., `images/php-command-shell.png`, `images/access-shell.png`, `images/license.png`) with the actual paths to your images in the repository.
- This Markdown file is structured to provide a comprehensive overview of the tool, installation instructions, usage examples, and ethical considerations, making it suitable for a GitHub repository.
