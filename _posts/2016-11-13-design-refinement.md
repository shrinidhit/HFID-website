---
layout: post
title:  "Design Refinement"
date:   2016-11-13
description: 2016-11-13
---

## Our Design
In this phase, our design evolved based on the feedback we received during the Design Development phase. Though our original timeline interface concept was not well received, we learned that users care a lot about the timing of tasks. We also learned that users value having a linear, step-based overview of the tasks they need to complete, though our step-based interface was also not well received. We decided to take the best features of both of these interfaces to create an entirely new one. As mentioned in the Design Development write-up, this interface features a linear progression of tasks represented by bubbles across the top of the page. There are larger bubbles for big tasks and smaller bubbles for the sub-tasks that need to be completed before them. The bubbles also have different colors to represent their states: black for incomplete, blue for in progress, green for complete, and gray for inaccessible (need to complete subtasks first).

<figure class="col l8 offset-l2">
	<img src="{{ '/images/acceptance_letter.jpg' | prepend: site.baseurl }}" alt="Digital Prototype Acceptance Letter"> 
</figure>

<figure class="col l8 offset-l2">
	<img src="{{ '/images/acceptance_letter_completed.jpg' | prepend: site.baseurl }}" alt="Digital Prototype Completed Acceptance Letter"> 
</figure>

## Changes

### Digital Prototyping Tradeoffs

While creating pages for our [digital prototype](https://invis.io/M399OC4K2), we realized that we only needed to design the steps up to the I-20 to receive useful feedback on our interface. This is because the steps are fairly repetitive and testing the process up to the I-20 will give us enough feedback on the core interaction. Additionally, creating pages for every single step in the process would be unnecessarily time consuming for us.


Another tradeoff is the flexibility in the digital prototype. When paper prototyping, we used a transparent sheet and a dry erase marker to easily and quickly represent almost any state the user could reach. In the digital prototype, it is a hassle to create a separate page for all of the possible states of the application, so we simplified down to one interaction path and made the walkthrough scenario very linear.

### Heuristic Evaluations

Based on our work in this phase and the feedback we received from the heuristic evaluations ([Casey]({{"/documents/casey-eval.html" | prepend: site.baseurl }}), [Christina]({{"/documents/christina-eval.html" | prepend: site.baseurl }}), [Deniz]({{"/documents/deniz-eval.html" | prepend: site.baseurl }}), [Jason]({{"/documents/jason-eval.html" | prepend: site.baseurl }}), [Patrick]({{"/documents/patrick-eval.html" | prepend: site.baseurl }})), we plan on making the following changes to [our prototype](https://invis.io/M399OC4K2):

**Create an Account**<br>
In our current prototype, the “create account” section is on the left hand side of the start page, and is called “Start New,” while the login section is on the right hand side. The “Start New” wording was confusing to our users, so we will change it to say “Create Account”. The “login” and “create account” sections were also too visually similar, and users were confused which was which. We looked at Facebook’s login/create account page, and realized we can make the login section visually separate by putting it in the title bar, while leaving the create account section on the main page.


**Username & Password Creation**<br>
Currently, there is an option to log in with an existing username and password in our prototype, but no way to create a username and password in the first place. Account creation is not fully fleshed out, as it only prompts the user for their nationality and dates of travel. This missing step was, understandably, confusing to users during our heuristic evaluations, so we will be adding it during the next phase.


**“Forgot Password” Button**<br>
Additionally, there is no “forgot password” option when logging into our application. This is standard functionality across applications with user accounts, and it’s absence was noted during our heuristic evaluations. While it seems unnecessary to prototype the actual functionality of this button, we plan on adding it to the login section to make it look more like a standard interface.


**Title Bar**<br>
We are adding a title bar to follow common web app standards. It is also to add more visibility - we want to show the user what application they are using, and under what account. The title bar will have the application name in the center, and the login account info on the right hand side, as seen in most apps.


**Buttons in Timeline**<br>
The buttons in our current prototype do not clearly indicate their state. It is hard to tell which ones are clickable, which ones are in progress, and which ones are complete. To fix this, we plan to change the design language to make it clear which ones are complete by putting a check in the circles and changing the ones in progress . Additionally, we will add hover states to the circles to show that they are clickable.


**Wordiness in Descriptions**<br>
The descriptions in the steps are currently very wordy and use complex words. As this is a tool meant for students who do not live in the U.S., it is very likely that english is not their first language. For this reason it is even more important to use language that will be accessible for all. We will use more common words, and simplify sentences.


**Ability to Remove Added Steps**<br>
On the School Requirements page, the steps differ depending on school, so we allow the user to add steps. To increase user control and freedom, as well as allow users to recover from error states, we are adding the ability to remove steps that were added by the user. This will likely be in the form of a menu that allows the user to edit or delete any additional steps.


**Task Name Visibility**<br>
To support recognition rather than recall, we will include a way for the user to view the name of each bubble task from any page. This will likely be implemented as displaying the name of the task when hovering on the bubble.


**Steps to Complete on Milestone Cards**<br>
In the heuristic evaluation, some of our evaluators noted a violation of the visibility into system status heuristic. It was hard to tell what the exact steps that needed to be finished to complete the milestone task were. This was because our navigation bar could not convey a lot of information due to space constraints. To fix this, on our milestone pages, we will add a list of steps that need to be completed first, which will map to the dots on our navigation bar. This will allow us to map the numbers on the dots to actual step titles improving the way subtasks are conveyed.

## Key Insights
We realized we didn’t look at inspirational designs as much as we could have. For example, the login page vs. a create account page was confusing in our prototype, but could have been resolved earlier if we had compared it to current websites’ log in/create account pages.


It was only once we designed the prototype on a computer that we realized details missing in our paper prototype. For example, we don’t have a state that indicates the state of the dot/step the user is currently on. Different people on our team had different ideas of how this would be represented, since we hadn’t previously talked about it. It was only after we made this prototype that we realized we had different ideas on this unspoken detail, and could come to a consensus.


We assumed some features didn’t need to be functional in our prototype, but this confused our users. For example, the dots didn’t actually allow a user to navigate between screens in our prototype, because we thought we could explain it as we were showing the prototype to them. However, our reviewers got confused because they expected it to be functional, and it broke their expectation. They spent more time commenting on this, and it prevented us from getting feedback on other parts of our app.

## Questions for Future
- Will the changes proposed in this heuristic evaluation solve the problems we’ve identified?
- Will people tire of using our app, especially since the steps are repetitive? How can we account for this in user testing? 
- How can we properly user test for someone using our app in a long term visa process? Our user tests capture how people use the app when they first open it, but this may not be completely representative of long term use.
- Is the dot timeline intuitive as a navigation? Will people understand how to use this to go from step to step?


## Effort Chart

|Person      | What They Did|
|---         |---|
|Haley       |Designed 2 screens, created landing page, heuristic evaluations|
|Shrinidhi   |Designed 2 screens, helped create master style in indesign, heuristic evaluations, scenarios script|
|Radmer      |Designed 2 screens, linked screens in invision, heuristic evaluations, helped w/ scenarios script|
|Franton     |Designed 2 screens, helped create master style in indesign, heuristic evaluations, designed and pushed the website|
|Aaron       |Designed 2 screens, created master style in indesign, heuristic evaluations|
