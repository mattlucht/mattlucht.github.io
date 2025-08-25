---
title: "Learning about clinical assurance"
author: matt
---

This week we've had some really good conversations around [clinical assurance](https://www.england.nhs.uk/long-read/digital-clinical-safety-assurance/), so I'm writing this post to share some of what we discussed, mostly to help me organise my thoughts, but hopefully it'll be useful for others too. It may get a bit wordy!  

Since joining NHS England one of the steepest learning curves has been around understanding what needs to be done to meet clinical assurance standards. There's also another aspect, solution (or technical) assurance, but that's something for another day. 

Previously, I’ve worked in places with some pretty robust governance processes. However, when there’s a potential impact to someone’s health and well-being, ensuring we don’t inadvertently introduce negative consequences is crucial. As a result, there’s a slightly overwhelming amount of evidence we need to provide in demonstrate that we're clinically safe, even for something as seemingly innocuous as sending an [invitation for a routine appointment](/2025/08/04/where-am-i.html#what-are-we-doing). 

## What is clinical assurance?

At the risk of Clinical Safety Officers (CSOs) reading this and burying their heads in their hands, thinking "why doesn't he still get it", I’m going to keep this high-level. 

Clinical assurance is split into two standards mandated under the [2012 Health and Social Care Act](https://www.legislation.gov.uk/ukpga/2012/7/contents).

### DCB0129 safety standard

The [DCB0129 standard](https://digital.nhs.uk/data-and-information/information-standards/governance/latest-activity/standards-and-collections/dcb0129-clinical-risk-management-its-application-in-the-manufacture-of-health-it-systems/) focuses on the technical build side of clinical safety – has the thing been built in a way that it’s not going to harm anyone. 

It ensures that the product has been designed and built in a clinically safe manner, considering the underlying code, business logic, and all technical components.

### DCB160 safety standard

The [DCB160 standard](https://digital.nhs.uk/data-and-information/information-standards/governance/latest-activity/standards-and-collections/dcb0160-clinical-risk-management-its-application-in-the-deployment-and-use-of-health-it-systems/) is focused on the deployment and use of the product – is there a risk of someone using the thing in a way that might harm someone.

It aims to identify any risks associated with its use, particularly in terms of user safety, processes, and training.

### The assurance process

In a nutshell, the assurance process for both the 129 and 160 aims to identify potential things that could go wrong, rating those risks based on likelihood and impact. Risks can be identified throughout the product development lifecycle, but typically happen at what is known as a 'hazard workshop'.

Once risks are identified, it then looks at what mitigating strategies might be put in place which may include technical solutions, training and guidance, or evidencing through user research that the right thing has been designed and built.  

## Challenges we're overcoming

Many existing assurance processes have been designed from a view of solutions being procured or developed externally and follow a more [waterfall-like process](https://en.wikipedia.org/wiki/Waterfall_model) where requirements are specified up front, the solution being designed and heavily documented, then following a linear process of being built, tested, assured, and then deployed.

For the products that we're working on within Digital Prevention Services Portfolio (DPSP) we have a team of CSOs who recognise approach this is at odds with [agile working](https://agilemanifesto.org/) and we've been coming together to look at how we can tailor the assurance approach.

### Changes to the approach

Having worked closely with the assurance teams for several months, we're each learning more about each other's respective needs, and we're continually trying to improve how we work together.

#### Earlier engagement

We’re now engaging with the assurance teams much earlier on in the process.

Instead of waiting for the hazard workshop at the end of the delivery cycle, we’re having conversations to identify potential clinical risks during initial scoping.

This earlier engagement, allows us to identify potential risks from the outset, allowing us to have those in mind when we’re designing, testing, and building the product.

#### Communicating changes

Agile teams are generally quite comfortable with change. Through user research, we may identify needs that we didn't know about at the start; tech spikes can prompt us to take a different approach, or when we put early iterations of a product in front of users, we might realise that it's not working as we expected.

We're fortunate to have autonomy to adapt our approach to best meet the needs of users.

I like [JP Rangaswami's](https://confusedofcalcutta.com/) response to [Paul Downey's](https://whatfettle.com/) original [post](https://x.com/psd/status/568324759521501184):

> _Agile: make it up as you go along. Waterfall: make it up before you start, live with the consequences_


<blockquote class="twitter-tweet"><p lang="en" dir="ltr"><a href="https://twitter.com/swardley?ref_src=twsrc%5Etfw">@swardley</a> apropos, albeit tangentially, some of your tweets today. And yes, I have been reading your stuff since about 06</p>&mdash; JP Rangaswami (@jobsworth) <a href="https://twitter.com/jobsworth/status/1302947431240400898?ref_src=twsrc%5Etfw">September 7, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

As we inevitably iterate our approach, we need to make sure that we're communicating changes appropriately. We're still exploring the best way for doing this.

There is documentation that is justifiably needed to evidence what is being built, and we've been trying to document our approach as we go. The use of [architecture decision records](https://github.com/NHSDigital/dtos-manage-breast-screening/tree/main/docs/adr) and [design histories](https://design-history.prevention-services.nhs.uk/screening-invite/) definitely helps. But things like scope documents and solution designs can quite quickly become out of sync, leading to some conversations where we've talked at cross purposes.   


#### Language

We're trying hard to keep the language we use consistent and unambiguous. Within the NHS, there is a lot of domain-specific terminology, which often gets turned into acronyms. The same is also true within product development teams. It's absolutely OK to stop a conversation and ask for clarity! 

#### Approach to testing

An area that is improving, but still needs some work, is around the approach for testing the code that has been written. Rather than having someone in the team who is solely responsible for testing, or a team that we pass the code over to to test, each of the developers on the team is [writing automated tests upfront](https://github.com/NHSDigital/bcss-notifications/tree/main/tests).

Each of the test suites has a high degree of code coverage, which gives us the confidence that everything is working as expected based on predefined acceptance criteria.

This is different to how testing has typically been done in the past, and with it being such a crucial part of proving that something is clinically safe, we understandably need to ensure that everyone is comfortable with the approach and has the same level of confidence.

## We're getting better, but there's more to do!

In summary, the more that we're working together, the better the process is becoming. There are definitely still things that we can improve, but in understanding the clinical assurance needs better, and talking openly about our collective ways of working, we're finding ways through the sticking points.