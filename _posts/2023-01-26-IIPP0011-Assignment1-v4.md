---
title: The Minimum Viable Product v3.1
date: 2023-01-26 16:00:00 
categories: [assignments, public administration, digital transformation]
tags: [agile, mvp, user stories] # always lowercase
---
# From the Complex Sprawling Nonentity (CSN) to the Minimum Viable Product (MVP)
 
Working in the public sector I have witnessed several large digital projects that have never really delivered. They often start with high ambitions, quickly accumulate masses of feature requests, and then attempt to built it _all_.

Usually after milestones have been missed, there will be a time of reflection and then, after descoping, the project is sanctioned to continue. Afterall, the investment of so much finance, time - and hopes and dreams - cannot be wasted. If ever this "Complex Sprawling Nonentity" (CSN) does deliver, too often is to an evolved user base who now need something rather different.

Instead, changing the focus to one of delivering a [Minimal Viable Product (MVP)](https://en.wikipedia.org/wiki/Minimum_viable_product) ensures something useful is delivered without too great an initial investment. The MVP then serves the function of eliciting user feedback which can be used to develop the product further - or bin it, if that is what the feedback says.

Like the CSN, the MVP draws on an understanding of what the user wants. However, this research is more penetrative, digging further into what the users actually need, what they do and, importantly, why. This information is often summarised in [user stories](https://www.gov.uk/service-manual/agile-delivery/writing-user-stories). By delivering a core requirement quickly - the [U.S. Digital Services Playbook](https://playbook.cio.gov/) states "no longer than three months from the beginning of the project" - the MVP addresses a [whole user need](https://apolitical.co/solution-articles/en/transforming-governments-website) in a timely way.

I am interested in exploring what MVPs look like in the wild, and in applying this concept to non-digital projects. In later iterations of this post (see the next sections or future posts), I will review real-world MVPs and apply the approach to address a CSN of my own - the way I approach assignment writing. Therefore, this first section of this post was created to address the following user story:

> As _an instructor_ I need to _observe my student's understanding of the MVP concept_ so that _I can determine their comprehension of the topic_

# A example MVP: alpha.gov.uk

> _NB: This section uses links to archived websites which will probably be slow to load_
{: .prompt-tip }

> As _a student of Digital Transformation_ I need to _describe the MVP of gov.uk_ so that _I can cement my understanding of the MVP concept_ 

The first release of the new website from Government Digital Service (GDS), [alpha.gov.uk](https://webarchive.nationalarchives.gov.uk/ukgwa/20111004104546/http://alpha.gov.uk/) was an MVP based on [user needs analytics of existing government digital services](https://web.archive.org/web/20120403153730/http://digital.cabinetoffice.gov.uk/2011/05/23/what-was-the-evidence-users-information-needs-and-analytics/). This effort identified that a candidate product would allow citizens to report a lost passport, search for the dates of national holidays, as well as linking to existing services on the "official" government website, [direct.gov.uk](https://web.archive.org/web/20050206042150/http://www.direct.gov.uk/Homepage/fs/en). 
<div style="text-align: left;"><figure>
<img src="/assets/img/direct.gov.uk_wayback_2004_04_30.png" alt="The direct.gov.uk website, accessed on web.archive.org" width="362" /> <img src="/assets/img/alpha.gov.uk_wayback_2011-05-11.png" alt="The alpha.gov.uk website, accessed on web.archive.org" width="310"/>
<figcaption>Left: The direct.gov.uk website. Right: The alpha.gov.uk website.</figcaption>
</figure></div>

The [prototype site](https://gds.blog.gov.uk/about-alpha/) offered a search option as its core function, where the existing direct.gov.uk, offered a list of links to different functions and departmental sites. To me, this is much like walking into a reception and going to a main desk to ask for help, rather than having to identify which of 20 or more desks is the correct one to approach.

<div style="text-align: left;"><figure>
<img src="https://cdn-images-1.medium.com/max/800/1*hJYxnfs6npD09IuX4606OQ.png" alt="Image from KDnuggets.com illustrating how each iteraction of a product should be a product in itself - i.e. if its a mode of transport, rather than iterating to deliver successive components of a car, each iteration delivers increasingly complex vehicles: skateboard, scooter, bike, etc." width="362" /><figcaption>Image from kdnuggets.com (<a href="https://www.kdnuggets.com/2018/07/minimum-viable-data-product.html">What is Minimum Viable (Data) Product?</a>) illustrating how each iteraction of a product should be a product in itself</figcaption></figure></div>

Once the service was running, [users could interact and provide feedback](https://gds.blog.gov.uk/2011/07/29/alpha-gov-uk-wrap-up/). Now, with the product _in their hands_, users could say what they really want to do and what the outcomes of those actions should be. All these inputs, from users and experts, are essential to developing the [next iteration of the service](https://web.archive.org/web/20111205164903/http://digital.cabinetoffice.gov.uk/2011/08/11/gov-uk-from-alpha-to-beta/).

By pushing out a live MVP so quickly, the GDS was opening itself up to [highly qualified criticism](https://web.archive.org/web/20120403153730/http://www.disambiguity.com/alphagov/) as well as potentially confusing their users. However, as a user who has waited years to access core digital services, I find such transparency refreshing. I also wonder if I should be using this approach more in my day job in data research. 

# MVPs in more complex settings

> As a _research scientist_ I need to _consider how the MVP concept could be applied to implementing digital AI transformations_ so that _I can understand if it could improve the value of my research effort_  

My day job is in researching the production of data in the public sector. A issue is that we always have more requests for products than could ever be developed in time. The traditional approach is to research and then build a solution for each product in turn. Stepping back from this approach, our team conceived of a method, using AI, that make the initial production of anticipated data requirements more efficient. We attempted to prove this approach by initiating the development (in 2019) of a scaled-down version of the solution - a naive-MVP (nMVP) if you like. This work encountered so many snags that it is still ongoing.

Our nMVP addressed just one customer data requirement. However, contained the functionality that enabled the solution to be turned to other customer requirements. As such, the solution was massively over-engineered for the single customer requirement. Further, because the "generic backbone" of the solution was AI, scaling down system complexity (e.g. less data or simpler algorithms) can (and did) result in useless results. Therefore, one of the biggest set-backs in this work has been the repeated lack of traction with decision-makers who, understandably, want to see successful outcomes from the work.

A coda to this case study is that an alternative AI approach, which launched out of the same initial research and at around the same time as our nMVP, has gained traction and is delivering value to a series of customers. This method does need to be re-engineered for each customer but could use the "generic backbone" to reduce this effort. In this instance, the potential customer of the "generic backbone" is internal and currently happy without the product we are offering. 

# MVP as direction-setter

> As a _would-be decision-maker_ I need to _articulate my remaining uncertainties about MVPs_ so that _I can seek deeper understanding through discussion and observation_ 

MVPs are clearly a superior approach to initiating progress towards a solution. There is, however, a degree to which they set the direction of progress such that decisions on each iteration of the product are biased by the nature of previous instances. This bias may result in some options never being explored. If the customer is served, this may be irrelevant. Of course, this issue exists with CSNs. Is there a moment, therefore, that the product that started as a MVP has become a CSN and its time to start over?

____
I have never read a leadership text before but have enjoyed Greenway and Schwartz on this topic