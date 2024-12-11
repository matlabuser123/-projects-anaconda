# -projects-anaconda

install_anaconda.sh                   # Main installation script
|
|-- README.md                          # Documentation with setup instructions
|-- .gitignore                         # Exclude logs, backups, and temp files
|
|-- config/                            # Consolidated configuration
|   |-- anaconda_config.json           # Unified configuration file (version, install path, etc.)
|
|-- logs/                              # Combined logs
|   |-- installation.log               # Logs with clear tags for different steps and errors
|
|-- helpers/                           # Auxiliary scripts for individual tasks
|   |-- downloader.sh                  # Handles downloading the Anaconda installer (with retries and checksum)
|   |-- verifier.sh                    # Verifies downloaded files' integrity
|   |-- helper_functions.sh            # Reusable functions for validation, cleanup, etc.
|
|-- backup/                            # Optional backup of configs
|   |-- config_backup/                 # Backup of critical configuration files
|
|-- tests/                             # Directory for testing the installation and logic
|   |-- test_installation.sh           # Verifies the full installation
|   |-- unit_tests/                    # Unit tests for core functions
|       |-- test_downloader.sh         # Test for downloader.sh functionality
|       |-- test_verifier.sh           # Test for verifier.sh functionality
|
|-- tmp/                               # Temporary files during installation
|   |-- anaconda_installer.sh          # Temporary Anaconda installer file
|   |-- install_pid.txt                # Prevents multiple simultaneous installations
