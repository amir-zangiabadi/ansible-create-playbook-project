# Ansible Project Structure Setup Playbook

[![Ansible](https://img.shields.io/badge/Ansible-✓-lightgrey.svg)](https://docs.ansible.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Docs](https://img.shields.io/badge/docs-passing-brightgreen.svg)](https://docs.ansible.com/)
[![GitHub issues](https://img.shields.io/github/issues/amir-zangiabadi/ansible-create-playbook-project.svg)](https://github.com/amir-zangiabadi/ansible-create-playbook-project/issues)
[![GitHub last commit](https://img.shields.io/github/last-commit/amir-zangiabadi/ansible-create-playbook-project.svg)](https://github.com/amir-zangiabadi/ansible-create-playbook-project/commits/main)

## Overview

This playbook automates the creation of a standardized Ansible project structure on your local machine. It prompts you for a project name—complete with input validation and a default value—and then builds an organized directory layout tailored for efficient Ansible project management. The playbook sets up inventory files for multiple environments and creates a fully scaffolded role directory complete with starter `main.yml` files.

## Features

- **Interactive Project Naming**: Prompts for a project name with default and validation, ensuring your project name is well-formatted.
- **Organized Directory Structure**: Automatically creates a main project folder with subdirectories for inventory and roles.
- **Multiple Environments**: Generates separate inventory files for production, staging, and development.
- **Comprehensive Role Setup**: Constructs a role directory with essential subdirectories (defaults, files, handlers, meta, tasks, templates, vars, and tests) and populates key ones with a starter `main.yml` file.
- **Permission Settings**: Sets appropriate permissions for directories and files to ensure smooth operation.

## Prerequisites

- [Ansible](https://docs.ansible.com/) installed on your local machine.
- Basic knowledge of Ansible and YAML.
- Git (optional), if you plan to version control your project.

## How It Works

1. **Prompt for Project Name**: When executed, the playbook asks for a project name, using a default (`myproject`) if none is provided and ensuring the input meets a valid format.
2. **Directory Creation**: It creates a dedicated project folder along with subdirectories for inventory and roles.
3. **Inventory Files**: It generates inventory files for production, staging, and development environments inside the inventory directory.
4. **Main Playbook File**: A `site.yml` file is created with initial content that ties in your project role.
5. **Role Directory Structure**: Within the roles folder, the playbook builds a detailed role directory including standard subdirectories and populates critical ones with a starter `main.yml`.

## Usage

1. **Clone or Download the Repository (if applicable)**:
   ```bash
   git clone https://github.com/amir-zangiabadi/ansible-create-playbook-project.git
   cd ansible-create-playbook-project
    ```


## Run the Playbook: Execute the playbook with the following command:
 ```bash
ansible-playbook ansible-create-playbook-project.yml
```

**Replace (`your_playbook_name.yml`) with the actual filename of your playbook.**

Follow the Prompts: Enter your project name when prompted, and the playbook will create your project structure accordingly.

## Customization
Feel free to modify the playbook to suit your project needs:

Change or extend the directory structure.

Update the contents of the main.yml files for more detailed configurations.

Adjust file permissions or validation rules as needed.

## License
This playbook is licensed under the MIT License. You are free to modify and share it according to your project requirements.

## Contributing

Contributions and feedback are welcome! Please open an issue or submit a pull request if you have suggestions or improvements.

-------------------------------------------------------------------------------------------------------------------------------------------------
This playbook is designed to simplify the initial setup of your Ansible projects, allowing you to focus more on configuration and deployment tasks. Enjoy!
