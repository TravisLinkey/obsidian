
2024-08-15 11:00

Tags: [[AWS]] | [[Identity & Federation]]

### Overview
Allows you to manage multiple [[AWS]] accounts at once.

The top-level [[Organization]] is called the `Root OU` (stands for Organizational Unit)

The Root OU is known as the `Management Account`.

### Details
You can have OUs within OUs.
    ie. You can have an `Human Resources` OU from within the `Developer` OU. etc.

### Key Concepts
- Special account role called [[OrganizationAccountAccessRole]]
- Two types of `Feature Modes`
    - [[Consolidated Billing]]
    - [[All Features]]
- [[Moving Accounts]]
- [[Service Control Policy]]
- [[Backup Policies]]

### References
- [[Week 1]]
- [[Permission Boundaries]]

