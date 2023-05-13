# Logkeeper
Logging-Service for UNIX based systems, made in shell

## Table of Contents

- [Logkeeper](#logkeeper)
  - [Table of Contents](#table-of-contents)
  - [Description](#description)
  - [Features](#features)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Configuration](#configuration)
  - [Contributing](#contributing)
  - [License](#license)
  - [Contact](#contact)


## Description

This project is a shell script that enables users to monitor a specific port of their choice. The script continuously captures and logs incoming and outgoing network traffic on the specified port, including details such as IP addresses, protocols, timestamps, and additional data. It provides users with a flexible and customizable solution for monitoring and analyzing network activity. The logged information is stored in a dedicated log file, allowing users to easily review and analyze the recorded data for troubleshooting, security auditing, or analysis purposes

## Features

Function: Initial Setup

    File: logkeeper.sh

This function performs the initial setup for the logkeeper script. It checks if the count file exists. If the count file exists, it executes the log menu. Otherwise, it initializes the setup process.
Function: Read Port Information

    File: logkeeper-printer.sh

This function reads the information about which port to listen to from the logkeeper-config file. It uses this information to monitor network activity on the specified port. The captured information is then saved to a new file named logkeeper-$date.log, where $date represents the current date. A new log file is created each day to maintain updated and organized logs. Each entry in the log file includes the date, timestamp, and a message associated with the logged network activity.
Function: Adjust Configuration Values

    File: logkeeper-writer.sh

This function allows users to adjust the values inside the logkeeper-config file. It is part of the main menu in logkeeper.sh. Users can modify configuration values related to the logkeeper script, such as the port to monitor or other settings. After successfully adjusting the values, the function returns the user to the main menu.
Function: Print Log File Values

    File: logkeeper-reader.sh

This function prints out specified values from the log file. Users can specify which values they want to print, and the function displays those values on the screen. Once the values are printed, users can choose to return to the main menu.
Function: Logkeeper Installer

    File: logkeeper-installer.sh

This function is responsible for setting up the logkeeper script. It creates a path for storing log files, ensuring that the necessary directories are present. Additionally, it generates and configures a service file, which allows the logkeeper script to run as a service in the background. Finally, it creates a count file, which is used to track the number of log files created.

These functions collectively provide the functionality to monitor and log network activity on a specific port, configure the logkeeper script, manage log files, and facilitate the installation process.

## Installation

Provide step-by-step instructions on how to install and set up your project. Include any dependencies or prerequisites that need to be installed beforehand. You can also provide example commands or scripts to facilitate the installation process.

## Usage

Explain how to use your project. Provide examples and demonstrate the different functionalities available. If there are command-line options or parameters, describe them here. You can include code snippets, screenshots, or gifs to illustrate the usage.

## Configuration

If your project requires configuration files or settings, explain how to configure them. Provide details on the purpose of each configuration option and how it affects the project's behavior. Include examples or sample configuration files if applicable.

## Contributing

Specify how others can contribute to your project. If you welcome contributions, provide guidelines for submitting pull requests, reporting issues, or suggesting improvements. Include any relevant information on coding styles, development environment setup, or testing procedures.

## License

Indicate the license under which your project is distributed. Mention any third-party libraries or dependencies and their respective licenses, if applicable. You can provide a link to the full license text in a separate file if necessary.

## Contact

Optionally, provide contact information or links to relevant resources where users can reach out to you for support, feedback, or further information about the project.

---

Feel free to adapt the sections and content according to your specific project needs. Including comprehensive and clear documentation in your README will greatly help users understand and use your project effectively.