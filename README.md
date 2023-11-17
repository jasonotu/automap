# AutoMap - NLP Security Control Mapping

AutoMap is an experiment to explore the feasibility of using Natural Language Processing (NLP) with sentence transformers to assist with security control mappings.

This notebook uses the [CSA CCM v4.0.7](https://cloudsecurityalliance.org/artifacts/ccm-machine-readable-bundle-json-yaml-oscal/) and [CIS v8](https://www.cisecurity.org/insights/blog/introducing-the-cis-controls-oscal-repository) catalogs in OSCAL format. They will need to be downloaded separately due to licensing.

The best performance seems to be when using the [all-mpnet-base-v2](https://huggingface.co/sentence-transformers/all-mpnet-base-v2) model from Hugging Face.

Sample output:
```
AIS-07 maps to CISC-16
Base description: Define and implement a process to remediate application security vulnerabilities, automating remediation when possible. 
Target description: Manage the security life cycle of in-house developed, hosted, or acquired software to prevent, detect, and remediate security weaknesses before they can impact the enterprise.

DSP-01 maps to CISC-3
Base description: Define and implement, processes, procedures and technical measures to protect sensitive data throughout it's lifecycle. 
Target description: Develop processes and technical controls to identify, classify, securely handle, retain, and dispose of data.

...
```
