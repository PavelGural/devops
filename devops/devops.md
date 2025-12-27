### SRE

*Цемны Лес*

SRE: Balance between development speed and reliability

? - SLO - 99.999: 1 request on 10.000 can be failed

Reason for the issue:
3 why

Distributed systems

Cron: many people set Cron on :00 - not good


### Non-functional requirements (any product)
- Availability – Ensuring the system is up and accessible as required (e.g., 99.9% uptime).
- Performance
- Scalibility
- Automation
- Disaster Recovery
- Observability
- Security
- Cost
- Maintainability

Additional (good to have):
- Compliance – Adherence to regulatory, legal, or organizational standards.
- Portability – The ease with which the system can be moved to different environments (e.g., cloud providers).
- Capacity – The maximum workload the system can handle.
- Resilience – The system’s ability to recover from failures and continue operating.


### Fuck-ups

*DOU DevOps*

1. different time zone: 
- app on the VM - EU time-zone
- app should be stopped 12 a.m. UK time-zone
Cron-job - app was stopped 1 hour earlier than planned.
2. Manual action -> remove production data
3. Admin IAM in AWS -> cryptomining in AWS, sharing creds in public git.
-  Now: if creds share in GH, GH will notify AWS, and AWS limits the User (not able to create Cloud compute resources).
-  Also, it was a case when AWS assisted to find a hacker who compromised the AWS account.
-  Set the limit on day in cost
-  Ask AWS to forgive the sum:
    * you will not possible to proceed business
    * you’re going to use AWS for a long time
    * ...
    *
    AWS forgives you in a lot of cases.
