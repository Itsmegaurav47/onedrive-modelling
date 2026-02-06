# Formal Modeling and Authorization Oracle for OneDrive (Personal Edition)

## Project Overview

This repository contains the formal model and Python implementation of an authorization oracle for Microsoft OneDrive's access control system (Personal Edition). The model uses a Capability-Based approach (Link-Mediated Access Model - LMAM) to capture sharing links, hierarchical inheritance, Personal Vault security, and state transitions. The oracle simulates access decisions (GRANT/DENY), and a comprehensive test suite validates the implementation.

## Project Structure

```
project31/
├── oracle.py              # Main implementation
│   ├── Data Classes       # User, Resource, Link, Context, OneDriveState
│   ├── Helper Functions   # is_ancestor, perms_effective, req
│   ├── Policy Predicates  # valid_link, vault_access, can_manage
│   ├── Permission Functions # direct_perms, inherited_perms, total_perms
│   ├── Authorization Oracle # decide_access, oracle
│   ├── Admin Operations   # create_link, add_user, delete_link, etc.
│   └── Test Suite         # run_all_tests, enerated by 
└── formalmodel.pdf        # Formal model specification
```



## How to Run the Code


python oracle.py

# The test suite will execute automatically and print results
```
