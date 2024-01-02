## Project setup
1. Create a new project: `poetry new news-blog`.
   1. Keep in mind that it creates a new folder.
   2. During the command run poetry will show the path to the virtual environment.
2. Specifying dependencies: If you want to add dependencies to your project, you can specify them in the `tool.poetry.dependencies` section.
Also, instead of modifying the `pyproject.toml` file by hand, you can use the `add` command.
3. Using your virtual environment in PyCharm:
   1. Click on Python button in the bottom right corner of PyCharm
   2. Interpreter settings
   3. Click Python Interpreter dropdown - Show all
   4. Click + button in the top left corner
   5. Environment - existing
   6. Click a button with 3 dots ...
   7. Paste the path to the virtual environment from item 1.ii.
   8. Open `bin` folder and click on `python` file
   9. Click ok buttons until you get back to your code
   10. Switching between interpreters makes PyCharm reload dependency list

## Additional Information
### Why do we need VE
Running `pip install *library name*` will install library globally (everywhere on ma' computer).
We don't always want this. Often we want dependencies to be installed for specific projects only.
Poetry by default installs dependencies in unique/separate virtual environments per projects.
These environments are allocated outside the project as mere folders.
If you type `poetry show -v` you'll get path to virtual env. You can open it via terminal (`open *path*`) of finder
