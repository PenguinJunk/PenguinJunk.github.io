---
title: Wardley Mapping
date: 2023-02-12 16:00:00 
categories: [assignments, digital transformation]
tags: [Wardely mapping, user needs, value chain, technological evolution] # always lowercase
author: pj
---
# A Wardley Map of the Local Authority Planning Portal
> Complete a Wardley Map for a government or university service/system of your choice. Please write a short statement (500-1000 words) about any insights doing this work revealed to you.

A Wardley Map is a way of describing a service or business. The map is anchored on the user of the service and demonstrates dependent components. The direction of the y-axis indicates the visibility of the component to the user, describing the value chain from those components that the user is least aware of or interested in to those that matter the most to the user. The x-axis describes the evolutionary stage of each component, from early, ***Genesis***, through ***Custom Built*** and ***Product (or rental)***, to late stage standardised ***Commodity (or utility)*** (the cheat sheet on Figure 17 of [Simon Wardley's Finding a path](https://medium.com/wardleymaps/finding-a-path-cdb1249078c0) gives the characteristics of each of these stages).

## Describing the value chain
![fig](/assets/img/Wardley_map_175.png){: .left w="250"}
![fig](/assets/img/Wardley_map_176.png){: .left w="250"}
I chose to map the planning portal used by local authorities to allow residents to find, view and respond to planning applications. From recollection, I identified that users would need to be able to `Search` planning applications, `Respond` to existing ones, `Track` and receive notifications about applications and `Submit` their own planning applications. These four services are most visible to users.

The `Search` function, which I considered at this point to be the most important, uses a `GIS` to allow search defined on a map. In turn this uses Land Registry (`LR`) data about property extents. The other functions (`Respond`, `Track` and `Submit`), require the users' account details and so need a customer relationship manager (`CRM`). In later iterations, I realised that address data (`AB`) would be required by both `Search` and the `CRM`.

The information about planning applications would be drawn from, and submitted to, some form of database (`Case DB` -> planning application database, `PADB`) and, knowing how most applications are submitted with documents, some form of document store (`Doc Store`). In later iterations, I realised that there was some coordination function required between `PADB` and `Doc Store`, and also the `LR` and `AB` data, and so added a manager (`Appl$^n$ Mgr` -> `PA Mgr`).

These data, along with the data for the `CRM`, the `LR` and `AB` would all require a `Data Store`. The `GIS`, `CRM` and `PADB` would also need `Compute` and both the `Data Store` and `Compute` require `Power`, all of which are largely invisible to the user.

## Iterating the value chain
![fig](/assets/img/Wardley_map_177.png){: .left w="250"}
![fig](/assets/img/Wardley_map_178.png){: .left w="250"}
I iterated over this map and in the process realised that I'd missed a vital component of the value chain: the `Website` through which all users would access the other components. I had some internal discussion about whether `GIS` was 'exposed' to the user and therefore at roughly the same  position in the value chain to the `Website` or simply is part of the `Website`.

As a preamble to adding in the x-axis, I attempted a rough grouping of components into the stages. Whilst none of the components seemed to fall under ***Genesis***, I felt that the most visible components (`Search`, `Submit`, `Respond` and `Track`), the `Website` and the `PA Mgr` (in the figure this is still `Appl<sup>n</sup> Mgr`) were all ***Custom Built***. I believed the components next along the value chain, `GIS`, `CRM` and the required data `LR`, `AB`, `PADB` (still `CaseDB` in the figure) and the `Doc Store`, were all at the ***Product (or rental)*** stage and the remaining components, `Compute`, `Data Store` and `Power` were all ***Commodities (or utilities)***. At this stage I also realised that I was conflating two different users - those who want to submit applications and those who want to know about or respond to existing applications. 

## Check in with reality
I decided to visit my local authority's planning portal and was rather surprised to discover two significant differences between my map and reality. The first was that the `Submit` function did not exist, and in truth I don't remember it ever existing. The second was that `GIS` was no longer available, although I know that this had been available somewhen in the last three years. After some exploration of the planning portal, I concluded that it is a much diminished service without the ability to search using `GIS`.

Moreover, I realised that there is a difference between what stage of maturity a component _should_ have, compared to the maturity it _does_ have when applied in this specific setting. For instance, I had thought of the `PADB` as a product - because databases are pretty standard things - but realised that in this setting it is probably still very much ***Custom Built***. Similarly, from my personal, although limited, experience of cloud services, I realised that neither `Data Store` nor `Compute` are ***Commodity (or utility)*** because there is still some upheaval in switching to a new provider.

After a little digging, I learned that there is work being undertaken to develop the planning service. [This has identified users of the service: citizens, property developers, local authorities and the tech market](https://dluhcdigital.blog.gov.uk/2022/01/21/modernising-planning-software-in-collaboration-with-councils-and-suppliers/), as well as [more detailed descriptions of how these users may use a digital planning service](https://dluhcdigital.blog.gov.uk/2022/06/28/digital-planning-reform-an-overview/). The focus of this reform is on the `Submit` service and [a few local authorities are trialling beta releases of this service](https://dluhcdigital.blog.gov.uk/2021/06/30/mhclg-launch-two-beta-planning-products/).

## The final map
![fig](/assets/img/Wardley_map_final.png)
The final map attempts to represent my understanding of the planning portal as it currently stands. I have left the `GIS` component in because I believe it is important to users. For this reason, I have defined it as exposed to the user (rather than being a dependency of `Website`), but this is now marked in grey because it is not present in the planning portals that most users have access to. Similarly, I have separated out the `Submit` service and indicated that this is required by a different user, and coloured these grey. My perspective is that whilst these components are not available in the live planning portal, they are available to a few users who have access to the beta releases and they provide very high value to users.

