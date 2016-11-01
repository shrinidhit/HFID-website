---
layout: post
title:  "Design Development"
date:   2016-10-19
description: 2016-10-19
---

## Process Overview
Last phase, we narrowed down our problem to assisting international and exchange students with the Visa process for entering the United States. This phase, we tried out multiple interfaces in order to find the elements of a design we could move forward with. To do this we created multiple paper prototypes and led users through similar tasks in the Visa process for each one. From these usability studies, we collected feedback and synthesized the results into a final design. We will summarize our findings below.

## Final Design

<figure class="col l8 offset-l2">
	<img src="{{ '/images/final_design_1.jpg' | prepend: site.baseurl }}" alt="Final Design"> 
</figure>

Our product is an interface to help manage the Visa application process for exchange students. It does not complete the application for the user. Rather, it provides information on deadlines, and the steps you need to take to complete your visa. The key features are:

-   ##### A step based approach
    Users wanted to see a simple left to right or top down progression of what they have to do for their visa, step by step. Our timeline prototype allowed users to jump around in a different order, but it was still used only left-to-right in testing. Our list prototype was also used only top-to-down.
    <figure class="col l6 offset-l3">
        <img src="{{ '/images/feature_steps.png' | prepend: site.baseurl }}" alt="Final Design Feature Steps">
    </figure>

-   ##### Detailed help on how to complete each step
    We learned from our timeline prototype that just giving the basic steps like acceptance letter or passport copy are not enough. Students want to see more information on what each of those mean, and how to complete them.
    <figure class="col l6 offset-l3">
        <img src="{{ '/images/feature_details.png' | prepend: site.baseurl }}" alt="Final Design Feature Details">
    </figure>

-   ##### Ability to see a high level overview
    Users wanted to move through the tasks in order quickly, just to see their entire process before they even started. We originally had the “done” or “checkoff” button be the central call to action for each screen, and realized this wasn’t the right priority. This prototype, each screen’s primary call to action is the “next” button.
    <figure class="col l6 offset-l3">
        <img src="{{ '/images/feature_next.png' | prepend: site.baseurl }}" alt="Final Design Feature Next">
    </figure>

-   ##### Dates are extremely important to see at all times
    Dates and deadlines are very important to our users, because it was universally ranked within the top 5 on our cardsortings (results explained in further detail below). This prototype shows dates for all tasks on the top bar, and a detailed description of suggested start dates in each task.
    <figure class="col l6 offset-l3">
        <img src="{{ '/images/feature_dates.png' | prepend: site.baseurl }}" alt="Final Design Feature Dates">
    </figure>

-   ##### Prerequisites are important, and must be visualized in an intuitive way
    Prerequisites were also universally ranked within the top 5 in our cardsorting results. Our timeline showed prerequisites, but in many places, and in a slightly more confusing way. This prototype tries a new visualization: small dots are prerequisites, leading up to big dots, which are the final forms. This allows the prerequisites to work with our step based approach, and we will have to do further testing to see if it’s a useful visualization.
    <figure class="col l6 offset-l3">
        <img src="{{ '/images/feature_prereqs.png' | prepend: site.baseurl }}" alt="Final Design Feature Prereqs">
    </figure>

## Cardsorting
In our card sorting exercise and in our usability test, Users showed they care a lot about the timing of tasks--when they should start them and when are they due--the context around tasks, how to complete a task, and what are the prerequisites of a task. Our design meets all of these by having a recommended start date and a deadline for each large task or milestone, by having lots of room on the expanding panel for a description of why this step is necessary and how to complete it, and by having a linear progression with size indicating that the larger bubble needs the smaller bubbles to be finished first.
<figure class="col l8 offset-l2">
    <img src="{{ '/images/cards.jpg' | prepend: site.baseurl }}" alt="Card Sorting">
</figure>

## Prototype One: Timeline
In our usability study with the timeline prototype, we tasked users to complete their I-20 form, which is the form an institution gives approving each user's study there. They completed a form to determine what Visa they needed and what path they should take to get it. Following that, the users were presented with a timeline containing tasks represented by cards. Cards could be clicked, and a information panel would appear at the bottom of the screen with more details. In the bottom panel, the user could check a box marked done to complete the task. Some tasks had prerequisites, and so if they clicked the card before the prerequisite tasks were completed, the done box would be replaced with an x preventing them from completing in.

From our usability studies, we found that there were many points of confusion with this prototype. First, users were confused on what the prototype's purpose was. Did it complete my application for me? Was it to walk me through the process or to keep track of where I was like a checklist? Second, the timeline page was overwhelming at first. Users spent a lot of time familiarizing themselves with layout before working on tasks. Part of that was also the confusion of how the bottom panel was connected to the cards on the timeline and whether the cards themselves were clickable. Finally, users also felt there was not enough context behind each task and too few details on how to complete them. Users did appreciate how start and stop dates were expressed, but they did not seem to care much about spacing along the timeline representing time.

<div class="row">
	<div class="col l6">
		<img src="{{ '/images/start_1.jpg' | prepend: site.baseurl }}" alt="Timeline 1"> 
	</div>
	<div class="col l6">
		<img src="{{ '/images/start_2.jpg' | prepend: site.baseurl }}" alt="Timeline 2"> 
	</div>
</div>
<div class="row">
	<div class="col l6">
		<img src="{{ '/images/start_3.jpg' | prepend: site.baseurl }}" alt="Timeline 3"> 
	</div>
	<div class="col l6">
		<img src="{{ '/images/start_4.jpg' | prepend: site.baseurl }}" alt="Timeline 4"> 
	</div>
</div>
<div class="row">
	<div class="col l6">
		<img src="{{ '/images/timeline_1.jpg' | prepend: site.baseurl }}" alt="Timeline 5"> 
	</div>
	<div class="col l6">
		<img src="{{ '/images/timeline_2.jpg' | prepend: site.baseurl }}" alt="Timeline 6"> 
	</div>
</div>
<div class="row">
	<div class="col l6">
		<img src="{{ '/images/timeline_3.jpg' | prepend: site.baseurl }}" alt="Timeline 7"> 
	</div>
	<div class="col l6">
		<img src="{{ '/images/timeline_4.jpg' | prepend: site.baseurl }}" alt="Timeline 8"> 
	</div>
</div>
<div class="row">
	<div class="col l6">
		<img src="{{ '/images/timeline_5.jpg' | prepend: site.baseurl }}" alt="Timeline 9"> 
	</div>
</div>

## Prototype Two: List of Steps and Chat Pairing
With our list-based and task-oriented prototype, we asked users to go through a sample Visa application that we had broken up into achievable steps. All the tasks necessary to complete the Visa form were on the left on the interface. When a user clicked on a task, the selected task would appear on the right and provide steps to complete it. Upon completion, the user could continue to the next step. If the user prefered to complete a task that was easier, rather than the one that was next, they could complete that one first, provided there were no prerequisites. Once a task was completed, a green check mark would appear next to it. If a user had a question, they could click on the chat icon in the lower right. This icon, when clicked, would open a chat window where the user could choose from people who had gone through a similar process and were available to chat. The user could then ask the person any questions, and once the issue was resolved, close the window.

In our studies using the list of steps prototype with assistance provided by pairing users at different stages in the process, we found that the task-based system was well-received, but users were not interested in the chat option. Users liked they could clearly see the tasks they had to complete. They also liked that while there was clearly a suggested order to complete them in, they could choose a step out of order if it seemed easier to complete. For steps that required a form be filled out, the form would auto-fill based on the information that the user put in. Users liked the because it made it much easier to fill out the form. Users were at first confused about the order in which the steps were placed, and so an important iteration would be to have the finished tasks on the top.

While our initial conversations with users seemed to point to a feature that would allow the user to connect with another person that had gone through a similar process, this ended up not feature that users were interested in. This may be in part because the users who had had someone help them knew the person that was helping them personally. Having a stranger help them with their form did not appeal to the users. Users were more likely to consult a FAQ, Google, or an administrator rather than the chat.

<div class="row">
	<div class="col l6">
		<img src="{{ '/images/list_1.jpg' | prepend: site.baseurl }}" alt="List 1"> 
	</div>
	<div class="col l6">
		<img src="{{ '/images/list_2.jpg' | prepend: site.baseurl }}" alt="List 2"> 
	</div>
</div>
<div class="row">
	<div class="col l6">
		<img src="{{ '/images/list_3.jpg' | prepend: site.baseurl }}" alt="List 3"> 
	</div>
	<div class="col l6">
		<img src="{{ '/images/list_4.jpg' | prepend: site.baseurl }}" alt="List 4"> 
	</div>
</div>
<div class="row">
	<div class="col l6">
		<img src="{{ '/images/list_5.jpg' | prepend: site.baseurl }}" alt="List 5"> 
	</div>
</div>

## Prototype Three: Chat
We also tested a chat/messenger based prototype with our users. Users were tasked to also complete up to their I-20 form. Users completed each task step by step as a narrator walked them through the task to complete. When forms or photos of documents were required, a input bubble would pop up allowing the user to add the image needed with the app also validating it to make sure it was correct.

However, in walking users through the prototype, like when we walked them through the timeline, users were confused whether the app was actually completing their application for them or just walking them through completing it. In addition, users questioned how far along they were in the process, which we did not show in our prototype.


## Key Insights from Initial Prototypes
In trying to produce a design that addresses our brief, we realized that people were not particularly fond of our chat pairing prototype. We were surprised by this, because in our initial round of user testing during the Needs Analysis phase, we heard from a few users that they liked to read blogs online by people who had been through the process before. People also seemed to generally react positively to the idea of connecting with other people going through the process at the same time as them.

When we asked users why they did not like this feature, they said that they did not trust random strangers who just happened to be using the app at the same time as them to answer their questions. They did not believe that these people would necessarily have enough knowledge to be able to help them with anything, since they also had not been through the process yet. One user said that they didn't want the app to be like a "social network." What we learned from this was that we were trying to solve two separate needs with one prototype, and those two needs didn't mesh together particularly well. While our user group might enjoy and benefit from a social network-type app, they do not want this to be a part of their Visa application process. The insight that we gained from this is that it is best to design for just one need at a time.


## Shortcomings
In our overall process (from needs analysis to now), we decided on a problem to solve based on limited knowledge of our users. We started out with a rough idea for our user group: immigrant families looking for schools for their children. After spending some time trying to find users to interview, we realized that this group would not be easily accessible to us. Given the time constraints of this phase of the course, we decided to pivot to a more accessible user group that was in the same vein as the first: international and exchange students going through the paperwork process for studying in the U.S. Because it took us a while to come to this realization and to pivot our target user group, we ended up with even less time than expected to interview users. The information that we collected was based on limited information from a small set of initial user interviews. Thus, the need that we had chosen to address and our initial ideas for solutions may not have been as strong as they would have been otherwise. We aimed to address this during the Design Development phase, adjusting our solution and possible implementations accordingly as we did user testing.

## Next Steps
Our initial prototypes helped us refine our key features. To summarize again, these are: using a step based approach, giving detailed descriptions on what each task is and how to complete them, and intuitively visualizing the key information of dates and prerequisites. We've planned some UIs for these, such as connected bubbles of various sizes. Our next step is to test these UIs and make sure they accomplish the goals for our key features.

We want to be careful with any roadblocks that could hinder us with this step. The paper prototypes that we created are written entirely in English with no option to change the language. This assumes that our users are sufficiently proficient in English, which may or may not be a reasonable assumption. On one hand, our user group does consist entirely of students, and typically English proficiency is a prerequisite for studying abroad in the U.S. On the other hand, this is not something that we specifically addressed during our user testing sessions in the Design Development phase, and is something that we should look into further moving forward.
