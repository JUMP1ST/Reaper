# Push Package to Reaper Repository

**Stage Name**: push-signed-package

**Description**: This stage copies the package from the `Input` repository to the `Reaper` repository, commits the changes, and pushes them to the `main` branch.

**Details**:

* **Tool Used**: Git
* **Command:**

```
cp /workspace/input-repo/package.tar.gz /workspace/reaper-repo/ && \
cd /workspace/reaper-repo && \
git config --global user.email "you@example.com" && \
git config --global user.name "Your Name" && \
git add package.tar.gz && \
git commit -m "Add Helm package" && \
git push origin main || { echo "Git push failed"; exit 1; }

```

**Possible Expansions**:

* **Detailed Commit Messages**: Include more details in commit messages.
* **Error Handling**: Enhance error handling and logging.
