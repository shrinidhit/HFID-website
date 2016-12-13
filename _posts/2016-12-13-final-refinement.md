---
layout: post
title:  "Final Refinement"
date:   2016-12-13
description: 2016-12-13
---

Navigating the visa process is a tiresome hurdle for many international students who come to the United States of America. The necessary information is often hard to find, unclear, and unfriendly. Our web app tries to make this process better for international students by clearly breaking down the visa process into manageable steps. We especially prioritize dates and deadlines because this was highly valued in user cardsorting.To accomplish this, we explored three methods: a list prototype, a timeline based approach, and a chat interface. In the end, we settled on a modified version of the list prototype, with increased visibility on how steps may relate nonlinearly (such as common prerequisites which don’t have to be done in order). This was based on the work we did in the [design development stage]({{ site.baseurl }}{% post_url 2016-10-19-design-development %}).

<figure class="col l8 offset-l2">
	<img src="{{ '/images/final_start_page.png' | prepend: site.baseurl }}" alt="Final Landing Page Design"> 
</figure>

Since the visa application process usually spans several months, our application needs to be able to store and save user progress. Given this requirement, our landing page includes options to either log in or create an account. Also, the user is probably unfamiliar to our Timeline application, so we also include a description of Timeline on this screen. 

We have three competing pieces of information on this page (log in, create an account, and description of our application), so we were unsure which layout would be least confusing for our users. We designed a usability experiment to see which design reduced the amount of time it took for a user to login and understand what the application was supposed to do. The [usability study results]({{ site.baseurl }}{% post_url 2016-12-09-usability-study %}) led us to choose this design: a title bar with a login button on the top right, and a two column layout underneath that has the description of the app on the left and the initial information for creating an account on the right. The login and continue buttons link away from the landing page, because we found that this reduced the amount of information users received to be manageable when initially visiting our app.

<figure class="col l8 offset-l2">
	<img src="{{ '/images/sevis_registration_completed.png' | prepend: site.baseurl }}" alt="Timeline Example Page"> 
</figure>

After logging into the app, the user is brought to our main timeline page. Under the title bar at the top is the timeline navigation bar. Each bubble in the navigation bar represents a task, with the size of the bubble mapping to the size of the task. The coloring of the button indicates the status of the task: green means complete, light blue means can be completed, dark blue means currently selected, and gray means inaccessible at this time. Underneath the navigation bar is the information panel; here the user can see the task with its description and steps that can be checked off as they are completed. Once all the steps are checked off, congratulations text and a continue button will appear at the bottom of the page. 

This design was selected from our work in the design development stage. The navigation bar was the product of reconciling the feedback on the timeline and list prototypes. The timeline was designed to easily show nonlinear prerequisites and deadlines, but people were using it in a stepwise manner anyway, just moving left to right. However, on the list prototype, people were confused about the order in which to accomplish tasks. Therefore, we settled on this design of the navigation bar, because it had the layout of the timeline, which spatially establishes an order for tasks to be completed, but also visualized the information hierarchy of steps from the list prototype.

We also wanted to allow users to clearly visualize their progress in the app. This was something we heard users wanted during early rounds of testing, and it satisfies one of Nielsen's Heuristics (visibility of system status). To address this, we designed the bubbles in the navigation bar to change color upon completion, as described above.

The information in the panel below the navigation bar is included to meet our user’s needs. Users were keen to see dates to start and finish tasks, and a description with steps on how to complete the task. With these needs in mind, we added the due date of each task, as well as a recommended start date, to the top right corner of each step. This consistency makes these dates easy to find. Additionally, we wrote the descriptions of the steps with our users in mind. Because our users are exchange and international students coming to the United States from other countries, there is a chance that they don’t have strong English skills. The descriptions are therefore short, straightforward, and use easy-to-understand language, avoiding jargon wherever possible.

## Shortcomings

Ideally dates would be more prominent and step names would be more visible in the timeline, based on previous testing results. Implementing some of our ideas is very difficult in InVision due to the need for both hover and click states on timeline tasks. In addition, currently the linking does not keep track of the completed state of the pages, which could be quite confusing.

## Future Work

From our usability testing, we learned that the title "F1 Visa Timeline" does not clearly represent the purpose of our app. No one knows what an “F1 visa” is unless they’ve already done their research, and the concept of a “timeline” as implemented in our app is not obvious. Were we to continue working on this app, we would come up with a better title that more clearly represents our app to a new user.

Also, actually coding a prototype would allow us to save progress and include hover states, which would provide a much more consistent user experience.

## Effort Chart

|Person      | What They Did|
|---         |---|
|Haley       |Made start page a/b prototypes; usability testing, writeup & markdown; 3 final prototype pages; prototype assembly in InVision; final presentation outline; helped with final refinement writeup|
|Shrinidhi   |Helped Haley with start page a/b prototypes, 2 final prototype pages, conducted and took notes for usability testing, helped with final refinement writeup|
|Radmer      |Made 3 final prototype pages, wrote the final refinement writeup, helped with final presentation|
|Franton     |Start page a/b prototypes, made master template, 3 final prototype pages, helped with final refinement writeup, Markdown to websit|
|Aaron       |Made master template (including navigation bar), finalized splash screen, created three final prototype pages, helped to assemble final prototype|
