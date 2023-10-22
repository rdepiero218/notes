###
Random config settings that I always forget about when setting up new computers.

## Jupyter Lab & Jupyter Notebooks in Chrome's App mode
Allows for Jupyter Lab or Jupyter notebook to be opened without all the browser stuff (looks like a standalone app)

First make sure you have a config file

### For Jupyter Lab:
```
jupyter lab --generate-config
```
Then to set it to open with Chrome in App Mode add the following to the top of 'jupyter_lab_config.py'
```
#------------------------------------------------------------------------------
# NotebookApp(JupyterApp) configuration
#------------------------------------------------------------------------------
c.LabApp.browser = '/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --app=%s'
```
### For Jupyter Notebook
```
jupyter notebook --generate-config
```
Then alter the following line in 'jupyter_notebook_config.py' and uncomment
```
c.NotebookApp.browser = '/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --app=%s'
```
