
2024-08-15 09:22

Tags: [[AWS]] | [[Identity & Federation]] | [[Active Directory]] | [[AWS Managed Microsoft Managed AD]]

### Idea
We may want our On-Prem Microsoft [[Active Directory]] replicated to [[AWS]] for reduced latency or in case [[Direct Connect]] or [[VPN]] goes down.

We need to establish trust between the [[AWS Managed Microsoft AD]] and [[EC2]]

### Solution
We will needc to create a Microsoft [[Active Directory]] on [[EC2]] to estabilsh trust between our On-Prem [[Active Directory]] and the [[AWS Managed Microsoft AD]].

Once created, we will establish a two-way trust relationship between the newly created AD on [[EC2]] and our [[AWS Managed Microsoft AD]].

We can then replicate our On-Prem [[Active Directory]] to this new instance, and it will serve as a proxy to the AWS Managed AD.

### References
- [[AWS Managed Microsoft AD]]

