# Ironhack Project

Natural Language Processing

## 🧹 Jupyter Notebook Hygiene (Required)

This project uses **nbstripout** to ensure that **Jupyter notebooks are always committed without outputs or execution metadata**.

This keeps:
- Git history clean
- Pull requests readable
- Merge conflicts to a minimum

Notebook outputs should **never** appear in commits or pull requests.

---

### One-time setup (per developer machine)

Install `nbstripout` and register it with Git:

```bash
pip install nbstripout
nbstripout --install
```

This repository includes a .gitattributes file at the root level that applies nbstripout to all Jupyter notebooks.

```
*.ipynb filter=nbstripout
```

> **Note:** Your first commit after running a notebook may fail.
> This is expected — `nbstripout` has cleaned the file.
> Simply run `git add .` and commit again.

