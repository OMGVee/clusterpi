# clusterpi
stuff for my raspberry pi cluster

### Ansible

- prepare a `Python3 virtualenv` and activate it:
```python3 -m pip install --upgrade pip```

```pip3 install virtualenv```

```pip3 install --upgrade setuptools```

```python3 -m virtualenv ansible/.venv```

```source ansible/.venv/bin/activate```

```pip install ansible```

- move to the Ansible Directory and test it out
```ansible all -i inventory -m ping -f 1```
