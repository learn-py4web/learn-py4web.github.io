# Unit 1: Installing py4web, and editing code

In this unit, we learn how to install py4web, and how to edit its files via Visual Studio Code, which allows for easy editing and debugging. 
You can also enable [GitHub Copilot](https://copilot.github.com/), which understands py4web pretty well, by enabling the [Copilot extension](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot) in VSCode.

## Resources

* [Anaconda Python](https://www.anaconda.com/)
* [Managing Python environments in Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)
* [py4web](https://py4web.com)
* [py4web source repository](https://github.com/web2py/py4web)
* [Visual Studio Code](https://code.visualstudio.com/)
* [git](https://git-scm.com/about)

## Videos

* [Installing py4web from git](https://youtu.be/hv3aEaT6ulI).  If you really want, you can also [install py4web via pip](https://youtu.be/DM8Yy4WdmJ4), but the recommended way for this class is to install it from source.
* [Editing in py4web](https://youtu.be/xnyNbR4a-sQ)

_Note: The installation video briefly mentions two minor bugs; these have been fixed already in py4web._ 

## VSCode Configuration Files

On my linux system, I use the following files to configure VSCode for py4web development (replace `/home/luca` with your home directory). The files are in the root py4web directory. 

### `launch.json`

```json
{
    "version": "0.2.0",
    "configurations": [
        
        {
            "name": "Python: py4web",
            "type": "python",
            "request": "launch",
            "program": "py4web.py",
            "args": [
                "run", "--errorlog=:stdout", "-L", "20",
                "apps"
            ],
            "console": "integratedTerminal",
            "justMyCode": true
        },
        {
            "name": "Python: File",
            "type": "python",
            "request": "launch",
            "program": "${file}",
            "justMyCode": true
        }
    ]
}
```
