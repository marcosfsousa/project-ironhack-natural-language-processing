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

