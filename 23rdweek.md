# 10th - 14th of October

Continuing on from my work from last week I finished the container image for the NTCG application and successfully implemented a script which would automatically update the certifications when the container is launched. Finally I started looking at the current configs for NTCG and thinking about how I could improve the way they are used. I started off by trying to remove the massive amounts of duplication in the configs. Then I started taking out the different settings that I might want to have easy access to and be be able to change depending on what env the application is being deployed in. I put made these values accessible through a configmap in my helm chart.

### Off the Job

I am currently working on the following courses and reading the following books:

- A Cloud Guru - AWS Solutions Architect
- A Cloud Guru - Red Hat Certified Systems Administrator
- A Cloud Guru - Certified Kubernetes Administrator
- Udemy        - Python: 100DaysOfCode
- Alan Hohn    - The Book of Kubernetes - Page 69
- [DevOps Roadmap](https://roadmap.sh/devops) - Understanding Different OS Concepts
