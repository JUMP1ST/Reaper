# ClamAV Scan

**Stage Name**: scan-clamav

**Description**: This stage runs ClamAV to scan the cloned repository for viruses.

**Details**:

* **Tool Used**: ClamAV
* **Command**:

```
clamscan -r /workspace/input-repo || { echo "ClamAV scan failed"; exit 1; }
```

**Possible Expansions**:

* **Custom Virus Definitions**: Use custom virus definition files.
* **Scan Reporting**: Generate and save scan reports.

