  # 6th - 10th of June
  
  This week my team started our 3rd sprint. The first task I picked up was IDT-8695: CI/CD pipeline for deploying all components. I picked this task up with Adam another apprentice as we felt it was quite a large task and we both wanted to get the experience of working on it. Prior to this sprint another colleague had already planned out a skeleton pipeline for use to base our pipeline off of, as seen below.
  
![Skeleton pipeline](https://github.com/OliverCutting/placement-diary/blob/main/5thweek-skeletonpipeline.png?raw=true)

From this we could see all the stages we needed for our pipeline and some of the neccessary requirements of it, such as making a test terraform workspace during the deployment stage unless the branch is main.

We made a good start and put most of the stages and requirements in however when we pushed the pipeline to gitlab, it got caught on the deployment stage, giving us an Access Denied error which unfortunately we were unable to resolve by the end of the week. The current yml file looks as follows.

![yml part1](https://github.com/OliverCutting/placement-diary/blob/main/5thweek-ymlp1.png?raw=true)
![yml part2](https://github.com/OliverCutting/placement-diary/blob/main/5thweek-ymlp2.png?raw=true)

## Off the job

This week for my off the job hours I have spent some time working on learning a new language. The language I chose was Go, this was because I know it is a very fast and efficient language often used in DevOps, and also often used to build DevOps tools. I started learning it by working through the Codeacademy: Learn Go course. I also spent some more time on Pluralsight making my way through the AWS Developer: Designing and Developing course. Finally I took the AWS Cloud Compute Skill Assessment where I was given the ranking of Proficient, and was also reccomended to watch the "Connecting with Amazon API Gateway" chapter of the Managing Applications in AWS course.

- Codeacademy - Learn Go
- AWS Developer: Designing and Developing
- AWS Cloud Compute Skill Assessment - 104 Proficient
- AWS Operations - 113 Proficient
- Managing Applications in AWS: Connecting with Amazon API Gateway

## Reflection

I suprised myself with this task so far as I believed I was going to struggle a lot more with the pipeline construction, I think doing this ticket as a pairing session helped to boost my confidence with it which is good. Hopefully we should be able to solve our issue early next week and then move onto another ticket.
