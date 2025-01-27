# Micro SaaS - Odoo Docker Instance Management
<img src="https://raw.githubusercontent.com/davidmonterocrespo24/odoo_micro_saas/15.0/micro_saas/static/description/0.jpg" alt="Imagen 1" width="800"/>
## Description

The **Micro SaaS - Odoo Docker Instance Management** module is a powerful and flexible solution for efficiently deploying multiple Odoo instances within Docker containers. Designed for businesses requiring an agile development and testing environment, along with the ability to manage several Odoo instances, this module simplifies development environment management and enhances collaboration in software projects.

## Key Features

- **Quick Instance Deployment:** Easily start and stop Odoo instances with a single click. The module automatically assigns available ports and clones repositories with the corresponding branches.
- **Repository Management:** Efficiently manage source code repositories. Associate Git repositories with each instance and control the branches used in each environment.
- **Custom Configuration:** Configure and personalize Odoo instances according to your needs. Each instance has its own odoo.conf configuration file, making it easy to tailor to your projects.
- **Activity Logging:** Maintain a detailed log of all activities related to instances, including starting, stopping, and restarting Docker containers. Simplify troubleshooting and event tracking.
- **Intuitive Views:** Enjoy intuitive and functional views that facilitate the management and monitoring of your instances. The Kanban view provides a quick overview, while the form view allows for detailed configurations.
- **Docker Compatibility:** Leverage the power of Docker for efficient container management. This module seamlessly integrates with Docker, ensuring optimal deployment and resource management.

## Key Benefits

- **Time Savings:** Reduce the time spent configuring and managing Odoo instances by automating repetitive tasks.
- **Enhanced Productivity:** Facilitate collaboration among development teams in software projects by providing separate and configurable development environments.
- **Complete Control:** Centrally manage and monitor your Odoo instances, maintaining a comprehensive record of activities.
- **Flexibility:** Easily adapt instances to individual project needs by customizing configuration files.
- **Scalability:** Scale vertically by adding new instances as needed, without complications or disruptions to existing projects.


##  Docker Compose Templates

- Define Docker Compose templates for Odoo instances.
- Each template has a name, sequence, and can be associated with tags.
- Templates include variables that can be customized when creating instances based on the template.

## Template Variables
- Define variables that can be used in Docker Compose templates.
- Variables can be of "Free Text" or "Field of Model" types."Field of Model" variables are used to extract values from Odoo records.

## Odoo Docker Instances
- Represent specific instances of Odoo running in Docker containers.
- Each instance is created from a defined template.
- Instances can have names, states (Draft, Stopped, Running, Error), HTTP ports, long polling ports, and more.
- Multiple templates can be defined, and when creating an instance, you can select an existing template and customize its variables.
- The instance can clone custom code repositories (e.g., Odoo modules) and configure a specific "odoo.conf" file for it.

## Core Functionality
- Create Odoo instances based on predefined templates.
- Customize specific template variables when creating instances.
- Manage ports to avoid conflicts.
- Start, stop, and restart Odoo instances through this module.
- Open the instance's URL in your web browser.

# TODO List
- [ ] Enhance the output of log messages for better readability and information.
- [ ] Move the functions for executing version control commands to a `/lib/git_utils.py` file for better code organization.
- [ ] Change the `branch` field of the `repository.repo` model to a new model as per project requirements.
- [ ] Implement enhancements to the `repository` model to enable operations such as clone, push, and pull on repositories.
- [ ] Create a scheduled task (cron) to automatically pull all repositories and rebuild instances with the latest changes. Ensure this task runs at desired intervals.

## Installation Guide

### Docker

To install Docker, follow these steps:

1. Visit the official Docker website for installation instructions: [Docker Installation Guide](https://docs.docker.com/get-docker/).
2. Choose the appropriate installation method for your operating system (Windows, macOS, or Linux).
3. After installation, verify Docker's successful installation by running `docker --version`.

### Docker Compose

Docker Compose simplifies the management of multi-container Docker applications. To install Docker Compose:

1. Follow the official Docker Compose installation guide: [Docker Compose Installation](https://docs.docker.com/compose/install/).
2. Select the instructions relevant to your operating system.
3. Confirm the installation by running `docker-compose --version`.

### Git

Git is a distributed version control system. To install Git:

1. Visit the Git website and download the appropriate installer for your OS: [Git Downloads](https://git-scm.com/downloads).
2. Follow the installation instructions provided.
3. Verify Git's installation by running `git --version`.

## Community Support and Contribution

We're thrilled to offer this module to the community as a free resource for efficient Odoo Docker instance management. We welcome contributions, feedback, and suggestions from the community to enhance and improve this tool further.

- **Contribute:** Help us improve this module by contributing code, reporting issues, or suggesting enhancements. Your contributions are valuable!
- **Star the Repository:** If you find this module useful, please consider starring the repository. Your support motivates us to continue development.
- **Spread the Word:** Share this module with your network and colleagues. Help us reach more users in the Odoo community.

Your support can help us create more features, improve stability, and make it even more valuable for users worldwide. Together, we can make a positive impact on the Odoo community and simplify development processes for all users.

Thank you for your support!

<!-- Imagen 1 -->
<img src="https://raw.githubusercontent.com/davidmonterocrespo24/odoo_micro_saas/15.0/micro_saas/static/description/1.jpg" alt="Imagen 1" width="800"/>

<!-- Imagen 2 -->
<img src="https://raw.githubusercontent.com/davidmonterocrespo24/odoo_micro_saas/15.0/micro_saas/static/description/2.jpg" alt="Imagen 2" width="800"/>

<!-- Imagen 3 -->
<img src="https://raw.githubusercontent.com/davidmonterocrespo24/odoo_micro_saas/15.0/micro_saas/static/description/3.jpg" alt="Imagen 3" width="800"/>

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=davidmonterocrespo24/odoo_micro_saas&type=Timeline)](https://star-history.com/#davidmonterocrespo24/odoo_micro_saas&Timeline)
