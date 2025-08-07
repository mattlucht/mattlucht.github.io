---
title: "Local government content discovery – week 6"
author: matt
---
Our focus for this week has primarily been around building a prototype for the "check if you qualify for money off your council tax" and "apply for money off your council tax" journeys.

## Mapping out the flows

The user journey flows that we started last week were based on an amalgamation of some existing forms used by each of the four local authorities. This gave us a good baseline to work from and helped frame a conversation to validate the purpose of each question. 

Working with Steph, our council tax subject matter expert, we were able to clarify why certain questions were needed and importantly we were able to remove some complexity by dropping questions that weren't really required.

If we were doing this work as a part of an actual council tax transformation project we could have spent a lot more time on this and within the journeys we've looked at there's definitely some complexity that we've purposely put aside. Maybe it's something for the future!

## Co-designing the content

With a good understanding of what information was needed from a user our next step was to figure out the order in which to ask for that information and how to best phrase those questions. As we mentioned last week, the goal was to only ask for information that's actually needed, no nice-to-have stuff, and to ask for the information in such a way that we'd be able to determine someone's eligibility as early on in the journey as possible.

Gwen led a content co-design session with Carolyn, Louise, Tom and Adrián.

The conversation really highlighted the nuances around seemingly simple things like how to determine the number of people living at a property. 

There was also the matter of how to ask about potentially sensitive circumstances such as when someone has recently died or when someone has separated from a partner.

![A screenshot of our content flows for the council tax prototype](/assets/images/content-flows.png)

There are definitely some bits to the journey where we still have questions, but the beauty of working in a fast and iterative way is that we don't need to solve all the problems at once, we'll learn through testing and figure out what needs to change. Don’t let [perfect be the enemy of good](https://en.m.wikipedia.org/wiki/Perfect_is_the_enemy_of_good) and all that!

## Building the prototype

As the questions and flows started to take shape we were able to begin building out the prototype.

We wanted the prototype to be available online so that we could put it in front of potential users and just 'real enough' that it was something that people could relate to.

There are some harsh edges to the prototype which has allowed us to keep it focused on the part of the journey we're working on. If it's useful and if there's appetite to do more work on council tax journeys the prototype can easily be extended.

![An animated gif of the council tax prototype](/assets/images/council-tax-prototype.gif)

Some minor tweaks aside, it's in a good place to start testing with users. To avoid any spoilers to potential research participants we'll share a link to the prototype after the next round of research.

### Prototyping toolkits

There are lots of different tools that can be used to help with prototyping. For our purpose we opted to use a modified version of the [GOVUK prototype toolkit](https://prototype-kit.service.gov.uk/docs/). Our rationale for using this was:

* the user interaction pattern for question branching (aka smart answers) has been tested many times over with users
* it's well documented and there's an active community of people using and maintaining the toolkit
* it's easy to host somewhere online (we’ve used Render)
* there's been extensive browser and device testing, so a reduced risk of web browser quirk tripping you up during user testing
* it's possible to do some subtle re-theming

On the point of re-theming, we made use of the modified toolkit from the Learn by making project. It's open source and available in a [public code repository](https://github.com/learnbymakingwales/lbm-prototype-kit) — another win for working in the open.

We've made the code for the council tax prototype open too, so having said that we won't share the URL to the clickable prototype just yet, if you really want to take a look [under the hood](https://github.com/learnbymakingwales/council-tax-prototype) here you go!
