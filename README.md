python33virtualenvwrapperforwindows
===================================

Just found out how to install virtualenvwrapper on windows
steps: 
1. download and install python33 on yoru machine
2. Add the python directory and pythondirectory/scripts to your PATH environment variable
3. download and install https://bitbucket.org/pypa/setuptools/raw/bootstrap/ez_setup.py using python ez_setup.py
4. download and install https://raw.github.com/pypa/pip/master/contrib/get-pip.py using python get-pip.py
5. run pip install virtualenvwrapper-win in commmand line or power shell
6. Start a command line!!!!!!! not a powershell, then use those commands:
7. Main Commands

mkvirtualenv <name>
Create a new virtualenv environment named <name>. The environment will be created in WORKON_HOME.
lsvirtualenv
List all of the enviornments stored in WORKON_HOME.
rmvirtualenv <name>
Remove the environment <name>. Uses folder_delete.bat.
workon [<name>]
If <name> is specified, activate the environment named <name> (change the working virtualenv to <name>). If a project directory has been defined, we will change into it. If no argument is specified, list the available environments.
deactivate
Deactivate the working virtualenv and switch back to the default system Python.
add2virtualenv <full or relative path>
If a virtualenv environment is active, appends <path> to virtualenv_path_extensions.pth inside the environment's site-packages, which effectively adds <path> to the environment's PYTHONPATH. If a virtualenv environment is not active, appends <path> to virtualenv_path_extensions.pth inside the default Python's site-packages. If <path> doesn't exist, it will be created.

resources:
for pip: http://www.pip-installer.org/en/latest/installing.html
for virtualenvwrapper-win: https://github.com/davidmarble/virtualenvwrapper-win/
