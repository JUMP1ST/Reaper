# Clone Input Repository

**Stage Name**: clone-input-repo

**Description**: This stage clones the `Input` repository from GitHub into the workflow’s workspace.

**Details**:

* **Tool Used**: Git
* **Command:**

```
git clone https://github.com/JUMP1ST/Input.git /workspace/input-repo && echo "Input repository cloned successfully" || { echo "Git clone failed"; exit 1; }
```

![](https://lh7-us.googleusercontent.com/docsz/AD\_4nXfeK-eL0HEWSiiUtoBejNJ-74UxefSTEnEW02Rypi44Nb0j5zbDhN0X3LmmBOcjOJ3pc8ZHV7BTif7SvUI7AkCnZGxE4arjgNBgSLebcOazllrDyvluDDZ97L4yTV8EblQS7qdTOVl2KD9bgsr\_9ett1s52?key=piJw1USgR6QyalXua2vW3A)



**Possible Expansions**:

* **Branch Selection**: Allow dynamic selection of branches to clone.
* **Authentication**: Use SSH keys or tokens for private repositories.

