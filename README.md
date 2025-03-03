# Django Project Setup (Windows)

## Prerequisites

Make sure you have the following installed on your system:

- [Python (latest version)](https://www.python.org/downloads/)
- [Git (optional, for version control)](https://git-scm.com/downloads)
- Virtual Environment (built-in with Python)

## Setup Instructions

### 1. Clone the Repository

Open **Command Prompt (cmd)** or **PowerShell** and navigate to your desired directory:

```sh
cd path\to\your\projects\folder
```

Then, clone the repository (if applicable):

```sh
git clone https://github.com/your-repo-name.git
cd your-repo-name
```

### 2. Create a Virtual Environment

Run the following command to create a virtual environment:

```sh
python -m venv venv
```

### 3. Activate the Virtual Environment

#### Command Prompt (cmd):

```sh
venv\Scripts\activate
```

#### PowerShell:

```sh
venv\Scripts\Activate.ps1
```

(If you get an execution policy error in PowerShell, run: `Set-ExecutionPolicy Unrestricted -Scope Process` and try again.)

### 4. Install Dependencies

Once the virtual environment is activated, install the required packages:

```sh
pip install -r requirements.txt
```

### 5. Run the Development Server

Start the Django development server: 

```sh
python manage.py runserver
```

or install the tasks extension and look down and build server to run the server

Your project should now be running at `http://127.0.0.1:8000/`

## Additional Commands

### Deactivate Virtual Environment

To exit the virtual environment, run:

```sh
deactivate
```

### Installing New Packages

If you need to install new dependencies, do so inside the virtual environment:

```sh
pip install package-name
```

Then update `requirements.txt`:

```sh
pip freeze > requirements.txt
```

## Troubleshooting

- **ModuleNotFoundError: No module named 'django'** → Ensure the virtual environment is activated before running Django commands.
- **'venv\Scripts\activate' is not recognized** → Ensure you're inside the correct project folder where `venv` was created.
- **PowerShell execution policy error** → Run `Set-ExecutionPolicy Unrestricted -Scope Process` and try activating the virtual environment again.

---



