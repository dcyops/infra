# INSTALL.md

## Installing Ansible

### Windows:

1. Create a Python3 virtual environment  
    `python -m venv ansible-venv`

2. Activate the virtual environment  
    `.\ansible-venv\Scripts\Activate.ps1`

3. Ensure pip, setuptools, and wheel are up to date  
    `pip install --upgrade pip setuptools wheel`

4. Install Ansible and dependencies   
    `pip install -r requirements.txt`

### Linux:

1. Create a Python3 virtual environment  
    `python3 -m venv ansible-venv`

2. Activate the virtual environment     
    `source ansible-venv/bin/activate`

3. Ensure pip, setuptools, and wheel are up to date     
    `pip install --upgrade pip setuptools wheel`

4. Install Ansible and dependencies  
    `pip install -r requirements.txt`