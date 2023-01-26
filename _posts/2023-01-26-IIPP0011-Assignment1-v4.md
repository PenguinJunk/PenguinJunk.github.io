---
title: The Minimum Viable Product v3.2
date: 2023-01-26 16:00:00 
categories: [assignments, public administration, digital transformation]
tags: [agile, mvp, user stories] # always lowercase
---
# From the Complex Sprawling Disappointment (CSD) to the Minimum Viable Product (MVP)
 
Working in the public sector I have witnessed several large digital projects that have never really delivered. They start with high ambitions, accumulate masses of feature requests, and attempt to built it _all_. Later, after milestones have been missed, there is a time of reflection and then, after descoping, the project is sanctioned to continue. Afterall, the investment of so much finance, time, hopes and dreams, cannot be wasted. If ever this "Complex Sprawling Disappointment" (CSD) does deliver, it is to an evolved user who now needs something rather different.

Instead, changing to an Agile approach and delivering a [Minimum Viable Product (MVP)](https://en.wikipedia.org/wiki/Minimum_viable_product) ensures something valuable is delivered without a great initial investment ([Schwartz, 2017 Ch3](https://itrevolution.com/product/a-seat-at-the-table/)). The MVP then elicits user feedback which can be used to develop the product - or bin it, if that is what the feedback says.

Both the CSD and the MVP incorporate user requirements. However, Agile demands more penetrative research that digs into what users actually need, what they do and, importantly, why. This information is often summarised in [user stories](https://www.gov.uk/service-manual/agile-delivery/writing-user-stories). By delivering a core requirement quickly - the [U.S. Digital Services Playbook](https://playbook.cio.gov/) states "no longer than three months" - the MVP addresses a [whole user need](https://apolitical.co/solution-articles/en/transforming-governments-website) in a timely way.

I am interested in exploring what MVPs look like in the wild. In later iterations of this post (next sections), I will review real-world MVPs. I will also apply the approach to address a CSD of my own - the way I write assignments. Therefore, this first section of this post was created to address the following user story:

> As _an instructor_ I need to _observe my student's understanding of the MVP concept_ so that _I can determine their comprehension of the topic_

# An example MVP: alpha.gov.uk

> _NB: This section links to archived websites which will probably be slow to load_
{: .prompt-tip }

> As _a student of Digital Transformation_ I need to _describe the MVP of gov.uk_ so that _I can cement my understanding of the MVP concept_ 

The first release of the new website from Government Digital Service (GDS), [alpha.gov.uk](https://webarchive.nationalarchives.gov.uk/ukgwa/20111004104546/http://alpha.gov.uk/) was an MVP based on [user needs analytics of existing government digital services](https://web.archive.org/web/20120403153730/http://digital.cabinetoffice.gov.uk/2011/05/23/what-was-the-evidence-users-information-needs-and-analytics/). This identified that a candidate product would allow citizens to report a lost passport, search for the dates of national holidays, as well as linking to existing services on the "official" government website, [direct.gov.uk](https://web.archive.org/web/20050206042150/http://www.direct.gov.uk/Homepage/fs/en). 
<div style="text-align: left;"><figure>
<img src="/assets/img/direct.gov.uk_wayback_2004_04_30.png" alt="The direct.gov.uk website, accessed on web.archive.org" width="362" /> &nbsp;<img src="/assets/img/alpha.gov.uk_wayback_2011-05-11.png" alt="The alpha.gov.uk website, accessed on web.archive.org" width="310"/>
<figcaption style="color: gray; font-style: italic;">Left: The direct.gov.uk website. Right: The alpha.gov.uk website.</figcaption>
</figure></div>

The [prototype site](https://gds.blog.gov.uk/about-alpha/) offered a search option as its core function, where the existing direct.gov.uk, offered a list of links to functions and departmental sites. The difference is like having a main helpdesk in a reception rather than having to identify which of 20 or more desks is the correct one to approach.

With the service running, [users could interact and provide feedback](https://gds.blog.gov.uk/2011/07/29/alpha-gov-uk-wrap-up/) about what they really want to do and what the outcomes of those actions should be. All these inputs, from users and experts, are essential to developing the [next iteration of the service](https://web.archive.org/web/20111205164903/http://digital.cabinetoffice.gov.uk/2011/08/11/gov-uk-from-alpha-to-beta/).

By pushing out an MVP so quickly, the GDS was opening itself up to [highly qualified criticism](https://web.archive.org/web/20120403153730/http://www.disambiguity.com/alphagov/) as well as potentially confusing their users. However, such transparency is refreshing. I should be using this approach more in my day job. 

<div style="text-align: left;"><figure>
<img src="https://cdn-images-1.medium.com/max/800/1*hJYxnfs6npD09IuX4606OQ.png" alt="Image from KDnuggets.com illustrating how each iteraction of a product should be a product in itself - i.e. if its a mode of transport, rather than iterating to deliver successive components of a car, each iteration delivers increasingly complex vehicles: skateboard, scooter, bike, etc." width="362" /><figcaption style="color: gray; font-style: italic;">Image from kdnuggets.com (<a href="https://www.kdnuggets.com/2018/07/minimum-viable-data-product.html">What is Minimum Viable (Data) Product?</a>) illustrating how each iteration of a product should be a product in itself</figcaption></figure></div>

# MVPs in a more complex setting

> As a _research scientist_ I need to _consider how the MVP concept could be applied when innovating with AI_ so that _I can understand how to improve the value of my work_  

My day job is in researching the production of data in the public sector. We always have more requests for products than could ever be developed in time. The traditional approach is to research and build a solution for each product in turn. Instead, our team conceived of a method, using AI, that would fast-track the initial production of anticipated data products. We attempted to prove this approach by developing a scaled-down version of the solution - a naive-MVP (nMVP) if you like. This work encountered so many snags that, after four years, it is still ongoing.

Our nMVP addressed just one customer requirement. However, it contained the functionality that enabled the solution to be turned to other customer requirements. As such, the solution was over-engineered for the single customer requirement. Further, because the "generic backbone" of the solution was AI, scaling down system complexity (e.g. less data or simpler algorithms) can (and did) result in a poor quality product.

A coda to this story is that an alternative AI approach, which launched out of the same initial research and at around the same time as our nMVP, delivered early and continues to deliver value to a series of customers. This method does need to be re-engineered for each customer but could use our "generic backbone" to reduce this effort. In this instance, the potential customer of the "generic backbone" is internal and currently happy without the product we are offering. I now appreciate how this is because our offering presents additional effort (as so plainly described in [Greenway et al., 2017, p156](https://www.andrewgreenway.com/book)).

# MVP as direction-setter

> As a _would-be decision-maker_ I need to _articulate my remaining thoughts about MVPs_ so that _I can seek deeper understanding through discussion and observation_ 

MVPs are clearly a superior approach to initiating progress towards a solution. They set the direction of progress such that decisions on each iteration of the product are conditioned by the previous iterations. This may result in some options never being explored. If the customer is served, this may be irrelevant. However, as a researcher I am intrigued by the implications of these unexplored directions of discovery. 

I realise that, without strict application of standards at each iteration, the MVP could easily develop into something akin to the CSD - a product that is increasingly difficult to maintain or develop. Of course, customers may drift away from the product before that happens, people and their wants and needs change, sometimes very rapidly.

The MVP sets a direction based on customers' requirements but it will also change the expectations and, ultimately, the requirements of those, and other, customers. The process is evolutionary. This must mean that one of the determinants of the long term success of any product developed using iterative, Agile approaches, is the MVP.