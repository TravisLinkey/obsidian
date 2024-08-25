
2024-08-15 09:14

Tags: [[AWS]] | [[Identity & Federation]] | [[Active Directory]]

### Overview
You can connect your on-prem [[Active Directory]] to [[AWS Managed Microsoft AD]]

- This requires you establish a [[Direct Connect]] (DX) or [[VPN]] connection

### Types
- One-way trust
    -- AWS => On-Prem
    -- On-Prem => AWS 

- Two-way trust (`Forest Trust`)
    -- AWS <=> On-Prem

### Details
[[Forest Trust]] is different than synchronization (replication is not supported)
    - Users exist independently (AWS and On-Prem users are different)

### References
- [[AWS Managed Microsoft AD]]
