# cogitate_tool

## Development Doc

### 1. File Structure

```bash
.
├── Pipfile
├── Pipfile.lock
├── README.md
├── scripts
│   └── cogitate.sh
├── src
│   ├── cogitate_tool.py
│   ├── data_collection.py
│   ├── demo.py
│   └── driller.py
├── tests
│   └── test_cogitate_tool.py
└── TODO.md
```

### 2. How to Use

#### 2.1 How To Install Packages

After pulling the repo, use `pipenv shell` in `cogitate_tool/` to enter the virtual
environment. Use `exit` to exit. Under the virtual environment, use
`pipenv install <package_name> --dev` to install new packages for development.

Here is a good [tutorial](https://realpython.com/pipenv-guide/) on how to use `pipenv`.

When under development, always install the virtual environment first by using
`pipenv install --dev`, then run the developing program by using
`pipenv run python program_name`.

#### 2.2 How to setup scripts

The purpose of script is to automate the running or testing process. To make the
scripts take effect, add the following code to the `Pipfile`:

```
[scripts]
command_name = "./scripts/script_name.sh"
```

Here the `command_name` is the command you want to use when running the project.
For example, if the `command_name` is `cogitate`, the we can use `pipenv run cogitate`.

### 3. CLI



### 4. PyDriller

The [homepage](https://github.com/ishepard/pydriller) and [documentation](https://pydriller.readthedocs.io/en/latest/intro.html) for `PyDriller`.

The available attributes can be found at their homepage.
