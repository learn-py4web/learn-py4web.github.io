# Unit 1: Installing py4web, and editing code

In this unit, we learn how to install py4web, and how to edit its files via either Visual Studio Code or PyCharm, two sophisticated Python editors. 

## Resources

* [Anaconda Python](https://www.anaconda.com/)
* [Managing Python environments in Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)
* [py4web](https://py4web.com)
* [py4web source repository](https://github.com/web2py/py4web)
* [Visual Studio Code](https://code.visualstudio.com/)
* [PyCharm](https://www.jetbrains.com/pycharm/) and [student licenses](https://www.jetbrains.com/community/education/#students)
* [Screenshot of run configuration for py4web in PyCharm](files/pycharm_py4web_config.png)
* [git](https://git-scm.com/about)

## Videos

* [Installing py4web from git](https://drive.google.com/file/d/1lvXXe0BJZ6pGzNxLXHgfX5upC0d9z41a/view?usp=sharing) ([YouTube](https://youtu.be/hv3aEaT6ulI)).  If you really want, you can also [install py4web via pip](https://drive.google.com/file/d/1y8ZS__6LiFTeTCSoqRkPSOQLZSxf9y9d/view?usp=sharing) ([YouTube](https://youtu.be/DM8Yy4WdmJ4)), but the recommended way for this class is to install it from source.
* [Editing in py4web](https://drive.google.com/file/d/1IDP5S7dA_igc73bwtch9vHOnZrMAJaQa/view?usp=sharing) ([YouTube](https://youtu.be/xnyNbR4a-sQ))

_Note: The installation video briefly mentions two minor bugs; these have been fixed already in py4web._ 

## VSCode Configuration Files

On my linux system, I use the following files to configure VSCode for py4web development (replace `/home/luca` with your home directory). The files are in the root py4web directory. 

### `launch.json`

```
{
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": "py4web",
            "type": "python",
            "request": "launch",
            "program": "/home/luca/py4web/py4web.py",
            "args": ["run", "apps"],
            "console": "integratedTerminal",
            "justMyCode": true,
        }
    ]
}
```

### `settings.json`

I have a Conda environment called `py4web` for py4web development. 
I installed the requirements via: `python -m pip install -r requirements.txt`
The code below is not strictly necessary, but it ensures that the correct python interpreter is used by default for this project. 

```
{
    "python.defaultInterpreterPath": "~/anaconda3/env/py4web/bin/python"
}
```