# 30th May - 3rd June

This week I continued working on my Dockerfile. I worked on putting the certificate inside of the dockerfile instead of mounting the certificate file to the container. I made this adjustment as with the certificate seperate it would need to be present on any computer trying to build the container, however the certificate couldn't be pushed to gitlab due to restrictions on the DWP gitlab preventing certain filetypes. The certificate was only needed for running the container locally anyway due to DWPs proxy setup so it didnt make sense to have a requirement for it to be present in any other format. Here is an image of the final draft of my dockerfile which I submitted a merge request for.

[dockerfile](https://github.com/OliverCutting/placement-diary/blob/main/4thweek-dockerfile.png?raw=true)

I made an effort to tidy up my commit history by squashing them and making sure the format of all the commit messages was correct before finally merging.

Due to this week only being 3 days long thanks to 2 bank holidays, it wasn't worth picking up a new big task so instead I spent sometime thinking about how a pipeline might work to build the container image. After some issues trying to get docker in docker to work I tried using a buildah script which had been setup by someone else within DWP and this script allowed the container to build successfuly. I also added in a second stage to the pipeline where I just printed out what python dependencies were installed in the container. This wasn't a requirement it was just moreso to demonstrate the pipeline working for people who come to edit it later.

## Reflection

I made a lot of improvement upon my previous dockerfile this week, however unfortunately due to it being a short week I didn't get time to work on my personal development.
