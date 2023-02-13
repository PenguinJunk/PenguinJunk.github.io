---
title: A Wardley Map of the Local Authority Planning Portal 2
date: 2023-02-13 11:00:00 
categories: [assignments, digital transformation]
tags: [wardley mapping, user needs, value chain, technological evolution, digital planning] # always lowercase
author: pj
---
> Complete a Wardley Map for a government or university service/system of your choice. Please write a short statement (500-1000 words) about any insights doing this work revealed to you.

A [Wardley Map](https://www.youtube.com/watch?v=Ty6pOVEc3bA) is a way of describing a service or business. The map is anchored on the user of the service and demonstrates dependent components. The direction of the y-axis indicates the visibility of the component to the user, describing the value chain from those components that the user is least aware of or interested in to those that matter the most to the user. The x-axis describes the evolutionary stage of each component, from early, ***Genesis***, through ***Custom Built*** and ***Product (or rental)***, to late stage standardised ***Commodity (or utility)*** (the cheat sheet on Figure 17 of [Simon Wardley's Finding a path](https://medium.com/wardleymaps/finding-a-path-cdb1249078c0) gives the characteristics of each of these stages).

# A best effort Wardley Map
I chose to map the planning portal used by local authorities to allow residents to find, view and respond to planning applications. From recollection, I identified that users would need to be able to `Search` planning applications, `Respond` to existing ones, `Track` and receive notifications about applications and `Submit` their own planning applications. In my [previous post](/posts/IIPP0011-Wardley-Mapping/), I described how I [initially defined the value chain of this service](../IIPP0011-Wardley-Mapping/#describing-the-value-chain) and how I [iterated over this to improve my understanding of value to the user, and stage of evolution of the components](/posts/IIPP0011-Wardley-Mapping/#iterating-the-value-chain).

Having iterated over early versions of the map, [I visited my local authority's planning portal](/posts/IIPP0011-Wardley-Mapping/#check-in-with-reality) and learned that the `Submit` component does not exist. However, this component has been identified as an important service and is [currently being developed and tested](https://dluhcdigital.blog.gov.uk/2021/06/30/mhclg-launch-two-beta-planning-products/) by a few local authorities. This initiative, now called [Open Digital Planning](https://opendigitalplanning.org/), is drawing on experience from an increasing number of local authorities and has brought in users at an early stage to develop the service in line with the [Local Digital Declaration](https://www.localdigital.gov.uk/what-is-the-declaration/). Rather than being just a service for accepting and filing application documents, the new service aims to [address the lack of clarity around making planning applications such that more applications are valid when they are received](https://dluhcdigital.blog.gov.uk/2022/06/28/digital-planning-reform-an-overview/). My conclusion was that, `Submit` is an essential component that should be exposed to the user. However, because it is only available to a few users at the moment, I have entered this component in as grey in the final map (below).

The other discovery, when visiting the planning portal, was that `GIS` is no longer available due to a worldwide vulnerability in a common technology used in the map (thank you to Emma Allen at Southampton City Council for the update). This component had previously enabled `Search` within regions defined on a map and, because people tend to be most concerned about developments that are geographically nearby, this component strikes me as very high on the value chain. The need to remove this component due to the vulnerability highlights another application of the Wardley map, in demonstrating the implications of having to remove a component. In terms of positioning `GIS` on the map, I did toy with putting it after `Website` in the value chain but decided (with some remaining uncertainty) to have this component more 'exposed' to the user because it is such high value. Again, because this is currently unavailable, I marked this in grey in the final map.  

![Final iteration of the Wardley Map as described in the text](/assets/img/Wardley_map_final.png)
_Final iteration of a Wardley Map of a local authority planning portal. See below for explanation of components._

---
> **Components**:  
`Submit`: Submit a planning application  
`Respond`: Respond to a planning application  
`Search`: Search for planning applications  
`Track`: Track planning applications (contains notification service)    
`GIS`: Provides mapping and ability to overlay geospatial data and define geographical regions for search  
`Website`: Interface between data and management components and the user  
`PA Mgr`: Planning application manager, handles the various tables and documents related to planning applications  
`PADB`: Planning application database, tables of data about planning applications  
`LR`: Land Registry data about property extents  
`AB`: Postal address data  
`CRM`: Customer relationship manager  
`Doc Store`: Storage for documents related to planning applications  
`Data Store`: Storage of data  
`Compute`: Processing of data etc.  
`Power`: Power required by compute and storage components  
---


# Further insights
This final version of the map is an attempt to represent what _is_ (in black) with an acknowledgement of what _should be_ present (in grey). The map also places components on the evolution axis in the position that I believe they fall in this particular service, despite some components, such as `GIS`, `PA Mgr` and `PADB`, having similar but more evolved components in other services. These components are likely to progress relatively quickly to the right, along with the `Submit` component, as Open Digital Planning develops. 

Indeed, most of the uncertainties I had when creating this map were with the evolutionary stage of the components. Several of the components, `Data Store`, `Doc Store`, `Compute` and `CRM` are so ubiquitous across public and private sector services that my initial inclination was to consider them a ***Commodity (or utility)***. However, experience suggests that these are all still very much at the ***Product (or rental)*** stage and that the service could not simply plug into an alternative supplier as one would with `Power`. For the user of these components (in this case, the provider of the planning portal service), this creates a cost of lock-in. To the supplier, this is beneficial but only until the market fully matures and standards emerge. The discussions of Wardley Mapping that I've experience, to date tend to recommend that more value can be extracted by the provider from components that fall at an earlier evolutionary stage. However, for the user (still the provider of the planning portal service), there is value in pushing for the evolution of these near-commodities to reduced the costs of use. Approaches that the user could take are demanding interoperability between elements of each component or participation in standardisation initiatives.

Considering the planning portal using Wardley Mapping has been very revealing. I started by assuming that there is only one user of the service and came to realise that there are [several different uses](https://dluhcdigital.blog.gov.uk/2022/06/28/digital-planning-reform-an-overview/) and thus users. The blog posts about Open Digital Planning highlighted how the pains of service users, particularly lack of clarity about the planning process, are a cost to the planning service because of time wasted dealing with invalid planning applications. 

A next phase could develop `Respond` to better enable citizen engagement in the planning process. I would hope to see similar effort to make relevant legislation, regulation, standards and advice intrinsic to this service, which would support the work of planning officers and panels. Intrinsic to this would be improvements to `Search`, to fully utilise the power of `GIS`, and `Track` to maintain citizen engagement in the process.  

