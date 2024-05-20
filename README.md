# Python venv Virtual Environment Cheat Sheet

## What is a Virtual Environment?
A virtual environment in Python is a self-contained directory that includes a Python installation and a collection of installed packages. It allows you to create isolated environments for different projects, ensuring that each project has its own dependencies and does not interfere with other projects. This is particularly useful when working on multiple projects that require different versions of the same packages.

## 1. Create a Virtual Environment
To create a virtual environment, navigate to the root directory of your project and run the following command:


`python -m venv qed-venv`


This command creates a virtual environment named `qed-venv` in your project directory.

## 2. Activate the Virtual Environment
Activating the virtual environment changes your shell's environment so that it uses the Python and pip executables installed inside the virtual environment instead of the global ones.

### On Windows:

`.\qed-venv\Scripts\activate`


### On macOS/Linux:

`source qed-venv/bin/activate`

After activation, your shell prompt will typically change to indicate that the virtual environment is active.

## 3. Install Packages
### Install a Single Package
To install a single package using pip, you can run:

`pip install <package_name>`

For example, to install the numpy library:


`pip install numpy`


### Install Multiple Packages
To install multiple packages using pip, you can run:


`pip install <package_name1> <package_name2> <package_name3> ...`


For example, to install some common data science packages:



`pip install jupyter matplotlib numpy pandas scipy scikit-learn`


Alternatively, you can use the following command, which ensures that pip is up-to-date:





## 4. Create requirements.txt
A requirements.txt file serves as a manifest of your project's dependencies, making it easier to recreate your development environment elsewhere. It includes a list of packages installed in your virtual environment along with their versions.



This file can be used to recreate the same environment elsewhere.

## 5. Deactivate the Virtual Environment
To deactivate the virtual environment and return to the global Python environment, run:


`deactivate`



## 6. Install Packages from requirements.txt
If you have a `requirements.txt` file and want to install all the packages listed in it, follow these steps:

- Place the `requirements.txt` file in the root of your project directory.
- Ensure your terminal is navigated to the project directory and your virtual environment is activated.
- Run the following command:

`pip install -r requirements.txt`

This command reads the `requirements.txt` file and installs all the packages listed, ensuring that your virtual environment has the same setup as specified in the file.

## 7. Delete the Virtual Environment
If you no longer need the virtual environment and want to delete it, simply remove the `qed-venv` directory.

### On Windows:
Open File Explorer, navigate to your project directory, and delete the `qed-venv` folder.

### On macOS/Linux:
Open your terminal, navigate to your project directory, and run:

`rm -rf qed-venv`


This will completely remove the virtual environment from your project directory.

## Summary
- **Create a virtual environment:** `python -m venv qed-venv`
- **Activate the virtual environment:**
  - *Windows:* `.\qed-venv\Scripts\activate`
  - *macOS/Linux:* `source qed-venv/bin/activate`
- **Install a single package:** `pip install <package_name>`
- **Install multiple packages:** `pip install <package_name1> <package_name2> <package_name3> ...`
- **Create requirements.txt:** `pip freeze > requirements.txt`
- **Deactivate the virtual environment:** `deactivate`
- **Install from requirements.txt:** `pip install -r requirements.txt`
- **Delete the virtual environment:**
  - *Windows:* Delete the `qed-venv` folder from File Explorer
  - *macOS/Linux:* `rm -rf qed-venv`

you can easily manage your` Python project's` `dependencies`, ensure a `consistent` development environment across `different machines`, and clean up when the virtual environment is no longer needed.







