# 42 Advanced Core - Monorepo with Submodules

The **42-advanced-core** repository serves as a central hub aggregating all repositories related to the *Advanced Core* curriculum at 42. Each project is included as a **Git submodule**, which enables modular organization and structured access.

---

## Repository Structure

Each subproject resides in its own directory and is tracked as a Git submodule. Example:
```
42_advanced-core/
└── scop/  # A submodule containing the 'scop' project
```

Navigation into any submodule provides access to its code, exercises, and resources.

## Cloning and Initializing Submodules

To clone the repository along with all submodules:
```bash
git clone --recursive <url>
```

If the repository was cloned without `--recursive`:
```bash
cd 42_advanced-core
git submodule init
git submodule update
```

This sequence downloads all submodules to provide access to the contained projects.

## Working with Submodules

Entering a submodule directory:
```bash
cd scop
```
Submodules can be explored, compiled, or executed according to the instructions in each submodule's README. Updating a submodule to the latest commit from its remote repository is performed with:
```bash
git pull
```

---

Each submodule contains its own README for project-specific instructions and guidance.
