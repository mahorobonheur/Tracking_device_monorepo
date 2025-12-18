# Tracking Device Monorepo
==========================

This repository contains the full Tracking Device project, combining both the backend and frontend applications as **Git submodules**.

## Repository Structure
=======================

tracking_app/
│
├── backend/ # Backend application (submodule)
├── frontend_app/ # Frontend application (submodule)
└── README.md

- **backend/**: Contains the backend API project.
- **frontend_app/**: Contains the frontend React application.

---

## Getting Started
==================

### 1. Clone the Monorepo
 ```bash
git clone https://github.com/mahorobonheur/Tracking_device_monorepo.git
cd tracking_app

```
2. Initialize Submodules
```   
git submodule update --init --recursive
```
This will clone the backend and frontend repositories into their respective directories.

Working with Submodules
=======================

To pull the latest changes from a submodule:
```
cd backend
git pull origin main
cd ../frontend_app
git pull origin main
```

*To commit changes to a submodule:*
-Make changes inside backend/ or frontend_app/.
- Commit in the submodule.
-Go back to the monorepo root and commit the submodule update:
```
git add backend frontend_app
git commit -m "Update submodules"
git push
```
Notes
=====
This monorepo uses Git submodules to keep backend and frontend projects independent but combined in one repository.

Make sure to always run git submodule update --init --recursive when cloning.





