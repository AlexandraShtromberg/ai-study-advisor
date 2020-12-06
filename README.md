# AI study advisor


## Summary
A study courses recommendation system for the Finnish universities will help students to create the study plan that they will enjoy and complete in the target period. 

Building AI course project

## Background
Students in Finnish universities have a lot of discretion in forming their minor and elective studies, regardless of their major. However, it is not that easy to form a curriculum especially if you are a fresher student and you do not have a wide network inside the university who can guide you in your choice. When I started my master studies in Aalto university, I faced the same challenge: several minors seemed appealing for me and I ended up changing minor in my study plan twice, which caused extra workload also for a study advisory at my school.

This topic is important not only from the perspective of a single student, but also for the whole university which funding might be dependent on the amount of credits a student has completed. Lack of sufficient information and recommendations on studies can lead to a situation when a student drops off the course when he or she realises that expectations on course workload or its connection to major studies were unrealistic.

In comparison with many other countries, Finnish system of education is flexible and many students work along with their studies. AI study advisor can also take into account student’s personal life circumstances when making a recommendation.

## Data and AI techniques

### Data
AI study advisor can rely on following data:
* Student feedbacks on completed courses
* Results of self-evaluation on the course main themes, workload and connection to other courses submitted by the course responsible professors and teaching assistants
* Course descriptions (including description of study methods and recommended literature)
* Course content (e.g. data scraping from Aalto University MyCourses platform)

### Techniques
* Nearest neighbour method can be used to identify most closest courses for each courses to build a recommendation system 
* Bag of words method can be used to process keywords for each of the course (order of words in the description does not matter as the fact that it has been mentioned, for example, when describing course prerequisites)

## How is it used?
Recommendation system will be embedded to the Oodi or another system where students can see course descriptions and create the study plans. End users will be opting in to use AI study advisor.

End users of the AI study advisor at the pilot phase can be study advisors who can verify that the recommendation model works correctly based on their own experience and “retrain” it by providing their feedback on relevance of recommendations. Retraining the model is very important as the initial model might lead to the situation that certain courses are always left out of the recommendation for example due to the course description being not updated in the Oodi system or lack of feedback answers (if course is new). Such a situation could gain a lot of negative feedback from the course professors and assistants.

Later, end users can be the students who create the study plan. There is a risk that students will rely on the recommendation system too much and thus be not too active in planning their studies but study advisors can mitigate them through follow-up sessions.

At all phases of the project, existence of a recommendation system will also motivate course staff to keep course descriptions up-to-date and detailed.

## Challenges
Project does not allow us to identify recommendations regarding new courses and/or old courses with updated descriptions and content. For certain programmes, like law, it might not be a big challenge, as the curriculum stays relatively stable. For other programmes, like big data analytics, it is more significant, as new technologies, programming languages and libraries emerge all the time. It can lead to a situation that courses that cover new technologies are ignored by the recommendation system.

System can also be biased for example by recommending just the easiest courses (as quite many easy courses gain a lot of positive feedback). It might be challenging to build a model that would identify such cases and it is important to consider what additional data inputs can balance the model.

## What next?
Project can grow by including more types of private and public institutions in their scope.

## Acknowledgements
There are some articles on this topic in the Internet - but they are against the paywall and cover foreign educational systems, so I decided not to research them and focus on my personal experience and perception of studying in Finland instead.

So, my acknowledgements go to Elements of AI course team for giving inspiration and to my employer for supporting digital upskilling journey.




