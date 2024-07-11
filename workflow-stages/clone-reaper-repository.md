# Clone Reaper Repository

**Stage Name**: clone-reaper-repo

**Description**: This stage clones the `Reaper` repository from GitHub into the workflow’s workspace.

**Details**:

* **Tool Used**: Git
* **Command:**

```
git clone https://github.com/JUMP1ST/Reaper.git /workspace/reaper-repo && echo "Reaper repository cloned successfully" || { echo "Git clone failed"; exit 1; }
```

**Possible Expansions**:

* **Branch Selection**: Allow dynamic selection of branches to clone.
* **Authentication**: Use SSH keys or tokens for private repositories.

