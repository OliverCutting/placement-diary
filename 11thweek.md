# 18th - 22th of July

This week I continued working on implementing kms encryption. In the end I sought help from Adam who was able to help complete the ticket. He done this by adding to the aws_kms_keys json policy, a section which granted the resource events.amazonaws.com the decrypt and generatedatakey permissions. We also added the following block of code which allowed us to add the current users aws details without hard coding them.

```data "aws_caller_identity" "current" {}

output "account_id" {
  value = data.aws_caller_identity.current.account_id
}```

### Off the Job

This week I continued working through the Solutions Architect Certification Prep course on A Cloud Guru and completed a number of practice questions. I also continued working on the Python 100 DaysOfCode challenge, the progress for which can be seen on my associated repo. I also spent sometime working through a Certified Kubernetes Administrator course and a Pluralsight Helm course as I know I will be working with these tools soon.
