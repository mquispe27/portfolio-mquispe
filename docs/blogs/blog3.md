---
title: UI Considerations in Hydrant
layout: doc
---

# Deep Dive Into Hydrant UI

After attending our lecture on UI design, I wanted to take a look at how these principles come into play in Hydrant, formerly Firehose, which is MIT's unofficial app for course scheduling.

## Consistency, Typography, Accessibility

![Hydrant](/../assets/images/Hydrant1.png)

In terms of consistency and typography, I find a nice color scheme with bright colors that each represent one class, and different themes including dark mode and high contrast mode that provide the same effect to the whole page for accessbility purposes. It's a nice touch to have a color coded legend to the top right as well.

## Information Scent

![Hydrant Information Scent](/../assets/images/Hydrant2.png)

In terms of information scent, the app is very informative and granular on every class, and easier to navigate than the official MIT course catalog. Just like how we saw that Amazon's catalogs give a little more information than Target's, in Hydrant we can not only see the professors and description and credits, but also helpful links to the course evaluations and even HKN's Underground Guide, which provides more specific feedback.

## Situational Context

![Hydrant Situational Context](/../assets/images/Hydrant3.png)

On second thought, a nitpick in consistency and situational context, is that while it clearly says in the bottom right what class you're looking at, the schedule's color does not change in the map reactively. You might expect a lighter or darker shade of blue when I am looking at 18.650, for example, but it does not happen. Regardless, for the search filters such as HASS and CI-H, they do fill as brown when selected. So something similar should happen for the classes, but it might be a deliberate choice by the developers for aesthetical purposes.

## Accelerators

Another thing we can glean from this image is that searching for classes, it autocompletes just like Google, and automatically loads based on the filters, so it definitely speeds up the process of finding a class compared to the official MIT course catalog, where you have to type your whole thing in and then click search.

![Hydrant Accelerators](/../assets/images/Hydrant4.png)

However, one thing I wish I could see is that in custom activities and events, which is a great feature on its own, I wish you could edit by dragging the event. Currently you can add a new time to an event by dragging on the calendar, but once you have a time, you can't move it around on the interface. You have to go to the clunky bottom right corner and manually remove a time and then draw the new one. This could be abbreviated from two steps into one step with the Google Calendar-like dragging of events, also clicking on the activity itself to rename it. However, since tracking extracurriculars is a secondary purpose of the app, I can see why this has not been a priority to be implemented yet.

## Fitts' Law and Error Tolerance

Expanding on this activity interface, it also takes time to scroll from the event to the time controls when you want to remove or add a new time. At the very least there is drag to add, because to fill in the tiny checkboxes for the days, is pretty pernicious. And when you're in a rush, "remove activity" and "rename activity" look very similar to the passing eye, and can be easily confused. You might want to change the name of the activity but end up deleting instead. The best thing to do here would be to add an "are you sure" prompt when clicking remove activity, common in many applications, or to make the remove activity button red to contrast easier, or to change "remove" to "delete" to make it less confusing. These would mitigate human biases.

There are more factors, but that is my look at the Hydrant application. Aside from the clunky event interface, Hydrant is an excellent app that will always take me through every semester at MIT.
