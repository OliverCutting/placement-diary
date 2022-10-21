# 17th - 21st of October

This week I attended a DevOps meetup for Integration within DWP at the Manchester hub where my team presented some of our recent work with our Kubernetes migration project. We also spent time discussing a recent failure within Integration which caused a system outage. We discussed how we operate in a blameless culture and how the bug which caused it was not the fault of the individual who pushed it, but of everyone within the wider team as it had went through multiple stages of review with no one seeing it. So the important thing to do is not to try assign blame but to try and see what we can all learn from teh issue and what we can do to prevent such issues from arrising again. We then spent time splitting into small groups with engineers we dont often work with to try and solve some problems which could benefit all of our workflows. My team personally worked on a solution which would prevent test infrastructure from fully going offline in the evening, allowing people hwho like to work late to still work. We accomplished this by uncovering the scheduled actions feature of auto scaling groups and finding a terraform module which teams can use to implement this feature in their workflows should they need it.

### Off the Job

I am currently working on the following courses and reading the following books:

- A Cloud Guru - AWS Solutions Architect
- A Cloud Guru - Red Hat Certified Systems Administrator
- A Cloud Guru - Certified Kubernetes Administrator
- Udemy        - Python: 100DaysOfCode
- Alan Hohn    - The Book of Kubernetes - Page 69
- [DevOps Roadmap](https://roadmap.sh/devops) - Understanding Different OS Concepts
