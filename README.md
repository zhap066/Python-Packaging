# Template repository for PH3010 Advanced Python

This is a template repository demonstrating how to package a python project. The directory is structured as follows:
```
template_project_PH3010_advanced_python/
├── .gitignore
├── LICENSE
├── README.md
├── pyproject.toml
├── requirements.txt
├── setup.cfg
├── .github/
│   └── workflows/
│              └── python_test.yml
├── docs/
│   └── ../
│   └── workflows/
├── src/
│   └── example_package/
│       ├── __init__.py
│       ├── command_line_interface.py
│       └── example.py
└── tests/
        └── test_example.py
```

Let's look at each element individually

* `.gitignore` contains files that should be ignored by git
* `LICENSE` the project license telling users who install your package the terms under which they can use your package
* `README.md` A [markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) document telling users about the project
* `pyproject.toml` tells build tools (like pip and build) what is required to build your project.
* `requirements.txt` contains the requirements for the project, you can install these with `pip install -r requirements.txt`
* `docs/` contains the documentation - we won't discuss this further here.
* `.github/workflows/python_test.yml` contains a [YAML](https://yaml.org/) file which determined how github Action are run
* `src/` contains the python package itself
* `tests/` contains the tests of the python package

*Description on how to install software*
The software to install can be found in setup.cfg. 

NOTE: INFORMATION IN NOTEBOOK NO LONGER WORKS DUE TO UPDATE IN PIP. FOLLOWING METHOD BELOW WORKS.

1. pip install --user . #This provides the path as to where 'python' is being accessed from [seen in yellow text]
>> WARNING: The script add_one.exe is installed in 'C:\Users\zhap066\AppData\Roaming\Python\Python38\Scripts' which is not on PATH.

2. python C:\Users\zhap066\AppData\Roaming\Python\Python38\Scripts\add_one.exe #This will error as a number is required next line will show argument example
>> add_one: error: the following arguments are required: number

3. python C:\Users\zhap066\AppData\Roaming\Python\Python38\Scripts\add_one.exe 2 #This can be any number, here I chose two. This will return 3
>> 2.0 add one is 3.0

4. add_one(2) #This will return the same as line 3, but from this point on in the code add_one() can be used as a shorthand. Must do the beggining section in order to use the function throughout
>> 2.0 add one is 3.0