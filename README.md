# Google Workspace License Manager

## Overview

Google Workspace License Manager is an open-source project designed to help administrators efficiently manage user licenses within a Google Workspace environment. This tool allows administrators to update user licenses based on groups and organizational units (OUs). It is being developed to fill the gap between terminal-based tools like GAM and a graphical user interface (GUI), providing a more user-friendly way to manage licenses.

This project leverages **OAuth 2.0** for authentication and is built with **Next.js** to provide a modern and interactive web interface.

## Features

- Assign and revoke licenses based on user groups and OUs.
- Generate reports on license usage and optimize costs.
- Support for multiple Google Workspace domains.
- Integration with Google Admin SDK for seamless management.
- Provides a GUI to simplify license management.
- Uses **OAuth 2.0** for secure authentication.
- Built with **Next.js** for a fast and dynamic front-end experience.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/Google-Workspace-License-Manager.git
   cd Google-Workspace-License-Manager
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Set up your Google API credentials:
   - Create a Google Cloud Project and enable the Admin SDK API.
   - Generate OAuth 2.0 credentials and download `credentials.json`.
   - Place the file in the project root directory.

## Usage

Run the tool using:

```sh
python main.py --assign --user=user@example.com --license=ENTERPRISE
```

Other commands:

- `--revoke` to remove a license.
- `--report` to generate a usage report.

## Configuration

Modify the `config.yaml` file to define license policies and automation rules:

```yaml
licenses:
  default: BUSINESS
  admin_group: ENTERPRISE
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Submit a pull request.

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

## Contact

For issues or feature requests, please open an issue on GitHub.

