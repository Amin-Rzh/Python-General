## How to setup Venv and Jupyter lab

1. Installing the jupyter lab:
   ```bash
      pip install jupyter lab.
   ```
2. Creating a new venv: 
   ```bash
      python -m venv {nameOfVenv}
   ```
3. Activating the venv:

   3.1. In Windows OS:
      ```bash
      {venv path}/scripts/activate
   ```
   
   3.2. In Linux OS:
      ```bash
         source {venv path}/scripts/activate
      ```
4. add venv to jupyter lab:
   4.1 be sure that your venv is already activated then use the following command:
   ```bash
      python -m ipykernel install --name={nameOfVenv}
   ```
   you should see the output:
   
      __Installed kernelspec {nameOfVenv} in {venv path}__
