# EspoCRM Instance

## Overview
This is an instance of EspoCRM 9.2.5.

## Installation Status

### Completed Steps
- [x] **File Permissions**: Set to `755` for critical directories (`data/`, `custom/`, `public/`, `application/Espo/Resources/`).
- [x] **Background Tasks**: Cron job configured for `cron.php`.

### Pending Steps
- [ ] **Database Configuration**: Needs a MySQL/MariaDB database and user.
- [ ] **Web Server Setup**: Point DocumentRoot to `public/`.
- [ ] **Installation Wizard**: Run via browser.

## Quick Start

1.  **Database**:
    ```sql
    CREATE DATABASE espocrm;
    CREATE USER 'espo_user'@'localhost' IDENTIFIED BY 'password';
    GRANT ALL PRIVILEGES ON espocrm.* TO 'espo_user'@'localhost';
    FLUSH PRIVILEGES;
    ```

2.  **Web Server**:
    Ensure your web server (Apache/Nginx) is configured to serve the `public/` directory.

3.  **Install**:
    Navigate to your server's URL and follow the installation wizard.

## Important Paths
-   **Config**: `data/config.php`
-   **Logs**: `data/logs/`
