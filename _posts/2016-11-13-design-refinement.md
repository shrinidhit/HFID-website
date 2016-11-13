---
layout: post
title:  "Design Refinement"
date:   2016-11-13
description: 2016-11-13
---

Based on our work in this phase and the feedback we received from the heuristic evaluations, we plan on making the following changes to our prototype:

#### Create an Account
In our current prototype, the “create account” section is on the left hand side of the start page, and is called “Start New,” while the login section is on the right hand side. The “Start New” wording was confusing to our users, so we will change it to say “Create Account”. The “login” and “create account” sections were also too visually similar, and users were confused which was which. We looked at Facebook’s login/create account page, and realized we can make the login section visually separate by putting it in the title bar, while leaving the create account section on the main page.


#### Username & Password Creation
Currently, there is an option to log in with an existing username and password in our prototype, but no way to create a username and password in the first place. Account creation is not fully fleshed out, as it only prompts the user for their nationality and dates of travel. This missing step was, understandably, confusing to users during our heuristic evaluations, so we will be adding it during the next phase.


#### “Forgot Password” Button
Additionally, there is no “forgot password” option when logging into our application. This is standard functionality across applications with user accounts, and it’s absence was noted during our heuristic evaluations. While it seems unnecessary to prototype the actual functionality of this button, we plan on adding it to the login section to make it look more like a standard interface.


#### Title Bar
We are adding a title bar to follow common web app standards. It is also to add more visibility - we want to show the user what application they are using, and under what account. The title bar will have the application name in the center, and the login account info on the right hand side, as seen in most apps.


#### Buttons in Timeline
The buttons in our current prototype do not clearly indicate their state. It is hard to tell which ones are clickable, which ones are in progress, and which ones are complete. To fix this, we plan to change the design language to make it clear which ones are complete by putting a check in the circles and changing the ones in progress . Additionally, we will add hover states to the circles to show that they are clickable.


#### Wordiness in Descriptions
The descriptions in the steps are currently very wordy and use complex words. As this is a tool meant for students who do not live in the U.S., it is very likely that english is not their first language. For this reason it is even more important to use language that will be accessible for all. We will use more common words, and simplify sentences.


#### Ability to Remove Added Steps
On the School Requirements page, the steps differ depending on school, so we allow the user to add steps. To increase user control and freedom, as well as allow users to recover from error states, we are adding the ability to remove steps that were added by the user. This will likely be in the form of a menu that allows the user to edit or delete any additional steps.


#### Task Name Visibility
To support recognition rather than recall, we will include a way for the user to view the name of each bubble task from any page. This will likely be implemented as displaying the name of the task when hovering on the bubble.


#### Steps to Complete on Milestone Cards
In the heuristic evaluation, some of our evaluators noted a violation of the visibility into system status heuristic. It was hard to tell what the exact steps that needed to be finished to complete the milestone task were. This was because our navigation bar could not convey a lot of information due to space constraints. To fix this, on our milestone pages, we will add a list of steps that need to be completed first, which will map to the dots on our navigation bar. This will allow us to map the numbers on the dots to actual step titles improving the way subtasks are conveyed.
