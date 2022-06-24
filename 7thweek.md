# 20th - 24th June

This week I worked on a few small tickets mostly based around the Makefile. The most interesting of which required me to add a make command to generate a local terraform workspace. It was required for this workspace to be named using the first 3 letters of the users first name and the first 3 of the users last name. This would be take from the users mac username which comes in the format first.last.

- oliver.cutting ---> olicut

This involved using regular expressions, which are things that I have used, however when I have used them previously I have found the regex needed online rather than writing it myself. This time around I was unable to find anything online for this specific use case. So I completed a tutorial on regexone.com on how to formulate my own expressions. Doing this allowed me to come up with the following.

`NAME := $(shell whoami | sed -E 's/([a-z]{3}).*\.([a-z]{3}).*/\1\2/')`

This code snippet uses the whoami shell command, then pipes it to sed -E where the regex ([a-z]{3}).*\.([a-z]{3}).*/\1\2/') is applied and then stored in the NAME variable. Essentially this regex takes the first 3 letters and saves it to a capture group 1, then says there will be any amount of any character followed by a full stop, then save the following 3 letters to a 2nd capture group, which will be followed by any amount of any character, finally returning capture group 1 + 2, i.e olicut.

## Off the Job

This week I spent a considerable amount of time completing the AWS Solutions Architect prep course on A Cloud Guru. I also started the 100DaysOfCode challenge on Udemy, starting on day 27 which had me create a simple GUI miles to km converter. All of my progress with 100DaysOfCode can be seen in my associated repo.
