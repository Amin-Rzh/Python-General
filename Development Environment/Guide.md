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
      python -m ipykernel install --user --name={nameOfVenv}
   ```
   4.2. you should see the following output:
   
      ```bash
         Installed kernelspec {nameOfVenv} in {venv configuration path for jupyter}
      ```
      
5. check the kernel.json file in {venv configuration path for jupyter}
6. see the list of installed virtual environments:
   ```bash
      jupyter kernelspec list
   ```
   
7. delete installed virtual environments:
   ```bash
      jupyter kernelspec uninstall {nameOfVenv}
   ```
