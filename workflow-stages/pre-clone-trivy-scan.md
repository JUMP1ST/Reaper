# Pre-clone Trivy Scan

**Stage Name**: scan-trivy-before-clone

**Description**: This stage runs a Trivy scan on the input repository URL to identify vulnerabilities before cloning.

**Details**:

* **Tool Used**: Trivy
* **Command:**\


```
trivy repo https://github.com/JUMP1ST/Input.git || { echo "Trivy scan failed"; exit 1; }
```

![](https://lh7-us.googleusercontent.com/docsz/AD\_4nXcho9D0XmiVKeFDsC3KlP3zea8ppvpVo62dWYRZxW1Owby-W832aiOTfrv8jaBKkqaPwVRU6Atf5V75HNjwLAyhScQVt1Xt4gss54qLmd0fLzy7kur0Gj565\_ktVJO1P0tegSlD\_nFJKb-54GGxCCDmkwM0?key=piJw1USgR6QyalXua2vW3A)



**Possible Expansions**:

* **Additional Scanning**: Integrate other vulnerability scanning tools.
* **Reporting**: Generate and save a report of the scan results.
