# k8s-sec-scan

The scripts use the Nmap, Kubescape, Checkov NVD Vulnerability Checker to preform the network and vulnerability scan on k8s cluster. 

## Table of Contents

- [Technologies](#technologies)
- [Features](#features)
- [Usage](#usage)
- [License](#license)

## Technologies

- k8s
- NMAP
- Kubescape
- Checkov
- NVD Vulnerability Checker
- Python
  
## Features

- It runs Kubescape to scan the cluster against the NSA/CISA hardening guide and saves the output in JSON format.
- It runs Checkov to scan the kubernetes manifests for misconfigurations and saves the output in JSON format.
- It requests the NVD API to get the latest kubernetes vulnerabilities and saves the output in JSON format.
- It gets the cluster IP address from the kubernetes configuration file and runs Nmap to scan the cluster IP address for open ports and service versions and saves the output in XML format.
  
## Usage
Can be executed directly from the command line.

```
git clone https://github.com/gma1k/k8s-sec-scan.git
cd k8s-sec-scan
python script.py
```

## License

[MIT](LICENSE)
