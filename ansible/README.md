# Ansible

- #### prepare a `Python3 virtualenv` and activate it:
  - `python3 -m pip install --upgrade pip`

  - `pip3 install virtualenv`

  - ```pip3 install --upgrade setuptools```

  - ```python3 -m virtualenv ansible/.venv```

  - ```source ansible/.venv/bin/activate```

  - `pip install ansible`

- #### test Ansible ad-hoc
  - `cd ansible`
  - ```ansible all -i inventory -m ping -f 1```
  
  at that point there should be some output like this:
  ```bash
  clusterpi1 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
  }
  clusterpi2 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
  }
  clusterpi3 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
  }
  clusterpi4 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
  }
  ```
