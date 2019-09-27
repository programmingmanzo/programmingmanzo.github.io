---
layout: post
title:      "Sinatra BodyImage App "
date:       2019-09-27 05:14:41 -0400
permalink:  sinatra_bodyimage_app
---


There is no better way to stay on track and be aware of progress other than logging it. I personally enjoy to work out and remain healthy, but it’s difficult to stay on track when you aren’t conscious of your progress or regression. I normally log all my body measurements and weight on paper, but sometimes I lose track of the notepad and start on a new one or just plain disregard logging anything.  

Attributing the benefits of logging, I deciding to build an app that would store all my measurements and keep them safe in one place. These critical points of measurement, which consists weight(lbs), waist(in), hips(in), right arm(in), left arm(in), right thigh(in) and left thigh(in) have been a great determinant of physique and health from personal experience. 

The app at the moment has very basic functionality. It allows for a user to sign up and log in. Once logged in a user can create an entry that includes critical points of measurement. Once your entry has been entered you have the ability to edit it or deleted it. You also have a page that will display all your measurements that you have entered by date and time, making it easy to keep track of progress. I would like to implement the ability to add a couple of images since, we as human beings we are very visual creatures. 

As far as the technical side, while creating the app, I encountered a few issues. One issue that had my mind in over drive had to do with the sending PATCH and DELETE requests. I continued to get Sinatra doesn’t know this ditty. I verified the path and it looked correct. Come to find out, the issue was that my Rack::MethodOverride that allows me to send requests other than GET and POST in the config.ru file was mounted under my controllers. Once I moved it above my controller that was going to use PATCH/DELETE requests it worked! Sometimes the issues are so simple! The other issues I encountered had to do with external CSS sheets. With so much reference material and help of cohort mates/cohort lead,  it’s a shame to spend too much time trying to debug. If you have spent a good amount of time trying to debug an issue, it is best to ask for help! Definitely something that I need to work on. Might be the engineer mentality!    

