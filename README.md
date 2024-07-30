# Overview

This document provides an overview and detailed explanation of the Helm Package Processing Pipeline. The pipeline automates the process of cloning an input repository, performing security scans, and pushing the results to another repository. It is designed using Argo Workflows and integrates tools such as Trivy and ClamAV for security scanning.

#### Key Features

* **Trivy Scanning**: Pre- and post-clone scanning for vulnerabilities.
* **ClamAV Scanning**: Scanning for viruses.
* **Git Operations**: Cloning repositories and pushing results.


Will update later with other various integrations
