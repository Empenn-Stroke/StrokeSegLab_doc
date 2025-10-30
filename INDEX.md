# StrokeSeg: Automated Stroke Segmentation Application

# ⚠️ This tool is for research purpose only!

# StrokeSeg: Automated Stroke Segmentation Application

StrokeSeg is a Python application designed to automate the segmentation of stroke lesions from medical imaging data. It provides a complete workflow including preprocessing, inference using trained models, and postprocessing with visualization tools. The modular architecture allows for easy customization and extension.

## Application Architecture Overview


The project is organized into several key modules, each responsible for a specific aspect of the stroke segmentation workflow:

- **entrypoints/**: Contains the main entry points for the application, including CLI and GUI interfaces.
- **preprocessing/**: Handles data preparation tasks such as brain extraction, resampling, and general preprocessing utilities (preprocessor.py, utils.py).
- **inference/**: Manages the inference process, applying trained models to input data for stroke segmentation (inference.py)).
- **postprocessing/**: Includes postprocessing steps (postprocessor.py) and visualization tools (viewer.py) to refine and display segmentation results.
- **managers/**: Provides configuration (config_manager.py) and option management (option_manager.py), as well as singleton patterns (singleton.py) for shared resources.
- **logger/**: Implements logging functionality (logger.py](./logger/logger.py)) to track application events and errors.
- **utils/**: Offers various utility functions for model management, file naming, path handling, string operations./utils/string.py, and more.
- **assets/**: Stores static assets such as images used in the application
- **logs/**: Contains log files generated during application runs.

Each module is designed to be modular and maintainable, facilitating easy updates and extensions to the application's functionality.

## User Guide

For detailed usage instructions, please refer to the [USER_GUIDE.md](./USER_GUIDE.md) file.

## Setup Instructions

To set up the application, simply run the provided setup script:

```sh
./setup.sh
```

You do not need to manually clone the repository; the `setup.sh` script will handle cloning automatically. If you have already cloned the repository, make sure it is located in a parent directory named `StrokeSeg.sh`, and execute `setup.sh` from the parent of `StrokeSeg.sh`. The script will update the repository and install all necessary dependencies for you.
