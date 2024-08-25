
2024-08-15 09:22

Tags: [[AWS]] | [[Identity & Federation]] | [[Active Directory]] 

### Idea
We may want our On-Prem Microsoft [[Active Directory]] replicated to [[AWS]] for reduced latency or in case [[Direct Connect]] or [[VPN]] goes down.

We need to establish trust between the [[AWS Managed Microsoft AD]] and [[EC2]]

### Solution
We will need to create a Microsoft [[Active Directory]] on [[EC2]] to establish trust between our On-Prem [[Active Directory]] and the [[AWS Managed Microsoft AD]].

Once created, we will establish a two-way trust relationship between the newly created AD on [[EC2]] and our [[AWS Managed Microsoft AD]].

We can then replicate our On-Prem [[Active Directory]] to this new instance, and it will serve as a proxy to the AWS Managed AD.

### Source Material
- [AWS Docs](https://docs.aws.amazon.com/directoryservice/latest/admin-guide/ms_ad_tutorial_test_lab_trust.html)

### References
- [[AWS Managed Microsoft AD]]

