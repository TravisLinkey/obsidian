
2024-08-15 11:51

Tags: [[AWS]] | [[Identity & Federation]]

### Overview
Defines a whitelist or a blacklist for [[IAM]] actions.

- Applies at the OU or Account level.
- Does not apply to the Management Account.

### Details
- Does not affect Service-linked roles
    - Service-linked roles enable other AWS services to integrate with AWS Organizations and can't be restricted by SCPs.

- [[SCP]] must have an explicit `Allow` from the root at each OU in the direct path to the target account. (Does not allow anything by default)

### Use Cases
- Restrict access to certain services.
- Enforce PCI compliance by explicitly disabling services.
- Use SCP to restrict creating resources without appropriate `Tags`
    - See: [[Tag Policies]]

### References
- [[AWS Organizations]]
