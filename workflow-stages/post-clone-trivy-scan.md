# Post-clone Trivy Scan

**Stage Name**: scan-trivy-after-clone

**Description**: This stage runs a Trivy scan on the cloned repository files to identify any vulnerabilities after cloning.

**Details**:

* **Tool Used**: Trivy
* **Command**:

```
trivy fs /workspace/input-repo || { echo "Trivy scan failed"; exit 1; }
```

**Possible Expansions**:

* **Detailed Reporting**: Generate detailed vulnerability reports and save them to a specified location.
* **Conditional Execution**: Execute only if the pre-clone scan is successful.



