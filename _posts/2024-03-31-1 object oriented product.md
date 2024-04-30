---
layout: post
title: Object Oriented Product
tags: Earning Growing Product
---

## tl:dr

1. **"Product" is a confused and contested term which causes problems** - It's fine to say there's no one right way to build great products and leave debates about form vs function to the internet but "Product" is, via definition and application, in danger of meaning so many things that it might mean nothing at all thus being either confusing or worse still impossible for companies trying to make great products and/or work at speed and scale.

2. **Here's why and how we got here** - A young (<20 years) discipline with one foot in the Agile Development Framework, one foot in the customer obsession needed for winning products and a head in the clouds of the companies that do both at speed and scale (M(F)AANG etc.)

3. **Here's a different way to think about it** - A surprisingly useful way of thinking about Product is as an entire software application or system, made up of multiple modules or packages - designed using OOP principles.  To deliver winning products make the objects model the real world problem space, think methods rather than functions and perhaps most importantly notice when switching from one building pattern to another.

4. **Why this might help** - A lot of the confusion and implementation challenges resolve if we think of the ability to respond to changing requirements, agility and flexibilty needed for great products as an emergent property of concepts like objects (built on 'Product' as a series of classes) that encapsulate both data and the operations that manipulate them. As with software engineering, this shift allows us to go beyond traditional functional approaches, also promoting modular design and reusability.

_Intro and Warning_: 
- A longer piece (hence, and apologies for, delay)
- Sundry jargon and multiple diagrams ahead

### Context

_**Airbnb**_ (_Figma config23 Conference_) : "... we got rid of the classic product management function. Apple didn’t have it either..."  
_**The internet**_ (_especially designers_): "Product management is dead!"  
_**1k+ Apple Product Managers\***_: "We exist"  
_**1m+ Product Managers\***_: "Is this about customer experience again?"  
_**250k + Product Owners\***_: "Wait, what?"  
(*_current job title on LinkedIn_)

**Airbnb** (_some time later_): "… well actually we kept the people, offloaded the programme management, combined it with marketing and called them something different… now they're Product Marketers"  
**The internet**: Wait, what?"

## 1. Problem - what is it and how is it done?

As suggested in the opening exchange, there is often a lot of confusion, tension and general fuzziness in discussions about product, product management and ownership, all the more surprising given the fact that well over 1m professionals on LinkedIn use it in their description of what they do.

The challenge is that when a word or concept is stretched to mean almost everything, it risks meaning nothing at all. As an excuse to include a favourite Aldous Huxley quote:

> "Words can be like X-rays if you use them properly -- they’ll go through anything... However, when words are overused or misused, they can become just background noise,..."

As somebody who has worked (and currently) in, at and on "product" (I'll drop the quotation marks as the point is made) for more than a decade, what follows is a brief overview and review as I see it.

Product is invoked when discussing:

- A Mindset ([https://medium.com/agileinsider/what-is-the-product-mindset-af06e01adf70](https://medium.com/agileinsider/what-is-the-product-mindset-af06e01adf70))
- A Set of Capabilities valuable to a segment ([https://www.gartner.com/en/information-technology/glossary/product-digital-business](https://www.gartner.com/en/information-technology/glossary/product-digital-business))
- An Operating Model ([https://www.svpg.com/the-product-operating-model/](https://www.svpg.com/the-product-operating-model/))
- A type of Engineer ([https://blog.pragmaticengineer.com/the-product-minded-engineer/](https://blog.pragmaticengineer.com/the-product-minded-engineer/))
- A Management Function ([https://www.productplan.com/learn/what-is-product-management/](https://www.productplan.com/learn/what-is-product-management/))


- Building on the LinkedIn current job titles theme we also have a range of what could be considered specialised versions of existing functions or roles:  
    - Product Manager (form of business management?)
    - Product Owner (form of scrum member)
    - Product Engineer (form of developer/software Engineering?)
    - Product Designer (form of design?)
    - Product Marketing Manager (form of marketing?)
    - Product Analyst (form of business analysis?)
    - Product Support Specialist (form of customer support?)
    - Product Co-ordinator (form of project management?)
    - Product Strategy Director (form of Executive strategy?)
    - etc.

So far, so confusing and so what?

It matters because, as opposed to start-ups who generally obsess over product (as outlined below in the Lean Startup) but can fail for adjacent, more interesting reasons - there are widely acknowledged challenges with introducing, transforming and executing 'Product' in large organisations. Today, many  claim to have switched to a "Product approach/mindset" yet still manage to manifest many of the habitual dysfunctions and pathologies common to their type and most importantly have no real idea why the switch hasn't delivered what was hoped for.

If no-one is quite sure what it means or understands exactly what product does, how do you introduce it? (especially in legacy businesses or market-fit stage organisations) - what are the necessary transformations - what needs to change? Why does executing a product driven approach not deliver great products faster?

As is obvious, this is often a complex multi-variate problem and way beyond the scope of one essay. However it is fair to say that the challenges with a less than twenty year old discipline began at it's inception.

## 2. Causes

The origin of the problems (in definition and application) can probably best be located 18 years ago (as of 2024) with Ken Norton in his essay "[How to hire a product manager](https://www.bringthedonuts.com/essays/productmanager.html)":

> **Remember friend, nobody asked you to show up**

> Product management may be the one job that the organization would get along fine without (at least for a good while). Without engineers, nothing would get built. Without sales people, nothing is sold. Without designers, the product looks like crap.

> But in a world without PMs, everyone simply fills in the gap and goes on with their lives. ... Now, in the long run great product management usually makes the difference between winning and losing, but you have to prove it. Product management also combines elements of lots of other specialties — engineering, design, marketing, sales, business development.

As he points out in 2023, this should have been entitled '_What_ is a Product Manager' and was written at the same time as Google were establishing their associate product manager program. He then summarises the qualities and by so doing begins to define the specific view of the problem space that the product manager works in if not their exact role - other than to ensure winning products in the long run.

The reason to have product managers at all in this sense, was thus to ensure winning (great) products driven by the success (and ability to deliver at scale and speed) of companies like those that the author worked at (Yahoo then Google\[Docs, Calendar, Maps and Ventures]).

The issue of whether 'product' is a discrete thing was then elegantly side-stepped in the Lean Startup (Eric Ries - 2011) by articulating a set of five principles for entrepreneurs to create a successful startup (which means you have a winning product - albeit not at scale) basically by beginning with customers (interviews, research, discovery), building an MVP (Minimum Viable Product) then testing and iterating quickly.

The 'build, measure, (validate) learn' loop located product squarely in the language/domain of software development reflecting the established agile approach of sprints and increments of value for building software - see below for Agile. (NB this is I think resolved in the conclusion)

The drive to instantiate this way of working in non-startups (Scale-ups and Established Enterprise) continued.  Marty Cagan's book "INSPIRED: How to Create Tech Products Customers Love" (2018) has as it's opening sales pitch:

> "How do today’s most successful tech companies—Amazon, Google, Facebook, Netflix, Tesla—define, design and develop the products that have earned the love of literally billions of people around the world? Perhaps surprisingly, they do it very differently than the vast majority of tech companies."

This at the time when a wider range of businesses were realising that by becoming 'Digital' they were de facto moving towards being a technology (if not a software) company. Naturally they then adopted a top down functional approach to organise and deliver.

Not surprisingly many diagrams followed, most famously Martin Eriksson, product leader  and founder of ProductTank in 2011 initially summed up product management using a simple [Venn diagram](https://medium.com/@bfgmartin/what-is-a-product-manager-ce0efdcf114c) that sits the product manager at the intersection of business, technology, and user experience.

![](https://kevanchristmas.github.io/public/assets/Eriksson_Product.jpg)

Further versions followed - notably the Atlassian Triad Model https://www.atlassian.com/blog/technology/engineering-team-structure centering Product Management in the "Business" role which moved it away from Engineering and in some ways made sense.

Made sense because, since the early 2000's the job of focusing on the business side of product development and spending the majority of their time liaising with stakeholders and the software engineering team had been elsewhere enshrined in the scrum team member called a Product Owner. (It almost certainly pre-dated 2000 as it was part of the Scrum Framework launched by Ken Schwaber and Jeff Sutherland).

In Scrum, the notion of "ownership" stems from the role's obligation to be solely accountable for maximizing the value of the product under development. The [Scrum Guide says](https://www.scrumguides.org/scrum-guide.html#team-po), in part:

> The Product Owner is the sole person responsible for managing the Product Backlog...The Product Owner is one person, not a committee...For the Product Owner to succeed, the entire organization must respect his or her decisions.

So, Product Manager == Product Owner?

Well, no. As the Ken Norton article/ Google experience from 2006 suggest, teams with Product Owners didn't always build winning products or at least could satisfy their roles where value was predominantly the delivery of working software. In general and for reference, Pendo's 2019 report based on an aggregation of anonymized product usage data (https://www.pendo.io/resources/the-2019-feature-adoption-report/) suggested that "80 percent of features in the average software product are rarely or never used" - further, "publicly-traded cloud software companies collectively invested up to $29.5 billion developing these features, dollars that could have been spent on higher value features and unrealized customer value". 

Product Management was still seen as the balancing act between building stuff right and building the right stuff. Of course we can show the roles and relationship in yet another diagram with circles: 

![](https://kevanchristmas.github.io/public/assets/Mojo_right_right.jpg)

This helps but still doesn't address the 'fuzziness' around the specific function of product nor how to approach delivery.

Product could clearly be represented as an open system with an output (Customer outcomes), comprising elements, interconnections, flows, feedback loops, leverage points etc.

Putting it together as a system of interconnected 'black boxes' such as Engineering, Business or even a level down toward a more gears-like (deterministically interconnected) understanding comprising Architecture, Research, Analytics etc. gets us so far but of course specifying excactly how these drive each other and which 'black box' they sit in, is where the complexity above begins necessitating a loose enough description or concept of Product that we could easily find ourselves at the beginning of this piece.

For (my own) reference I work with:

> Product is a system of geared concepts oriented to delivering maximum value exchange between a company and it's customer.

> A series of guided (by principles/approach) trade-offs (intersections) executed (by a system comprised of processes and functions) to optimise the value exchange between a company and its actual or desired target (creating and keeping) customers.

This contains some but not all of the (imho) important enough ideas.

There is also ongoing development around the ideas of two forms of Product Management  – for two very different situations: [feature teams vs product teams](http://www.svpg.com/product-vs-feature-team).

Very useful in so far as Product team> Feature team> Delivery team but we seem to still be in a world of defining functions or at least functional approaches.

The dilemma is well addressed in Melissa Perri's book "Escape the Build Trap":

> "To stay competitive in today's market, organizations need to adopt a culture of customer-centric practices that focus on outcomes rather than outputs. Companies that live and die by outputs often fall into the "build trap," cranking out features to meet their schedule rather than the customer's needs."

Customer-centricity and outcome focus seems to be moving us back in the direction of the 'core' Lean Startup approach and the companies that embodied it.

With a slight shift in thinking this could represent the penultimate stage to what might be the best way of representing Product.

Here, a model from a different discipline (perhaps not that different - we may just be adding to the Agile foundations borrowed from Software Development...) could be surprisingly useful.

## A different way to think about it

_(caveat - I wish to extend apologies in advance to CS graduates, IT professionals and fellow [Hyperskill](https://hyperskill.org/tracks/2) alumni where I first encountered the following..)_

OOP (Object Oriented Programming)

At it's simplest, OOP means trying to organise the code for your application or system into objects that model parts of your problem.

It was developed as a different approach to what is known as Procedural programming.

Below are some of the differences between procedural and object-oriented programming: 
(edited from https://www.geeksforgeeks.org/differences-between-procedural-and-object-oriented-programming/)
|Procedural Oriented Programming|Object-Oriented Programming|
|---|---|
|1. In procedural programming, the program is divided into small parts called _**functions**_.|In object-oriented programming, the program is divided into small parts called _**objects**_.|
|2. Procedural programming follows a _**top-down approach**_.|Object-oriented programming follows a _**bottom-up approach**_.|
|3. Adding new data and functions is not easy.|Adding new data and functions is easy.|
|4. In procedural programming, overloading is not possible.|Overloading is possible in object-oriented programming.|
|5. In procedural programming, the **function is more important than the data**.|In object-oriented programming, **data is more important than function**.|
|6. Procedural programming is based on the _**unreal world**_.|Object-oriented programming is based on the _**real world**_.|
|7. Procedural programming uses the concept of **procedure abstraction**.|Object-oriented programming uses the concept of **data abstraction**.|
|8. Code **reusability absent** in procedural programming,|Code **reusability present** in object-oriented programming.|
|**Examples:** C, FORTRAN, Pascal, Basic, etc.|**Examples:** C++, Java, Python, C#, etc.|

Without provoking internecine wars, it should be remembered that procedural programming is widely used and many applications are not 'object-oriented' but simply written in imperative style. 

A procedural style is best used when you have a very well specified problem, the specification won't change and you want a very fast running program for it. In this case you may trade the maintainability for performance.

This isn't meant as a comparison of pro's and con's but some key themes do stand out (even if not a directly similar usage) and suggest this is a worthwhile model for thinking about product.

Picking just four of the key ideas:

Objects vs Functions
Bottom up vs Top Down
Real world vs Unreal world
Data > Function





The approach to begin solving for the challenges outlined at the start would be to understand where a procedural pattern is being applied and try to switch it.

However, when it comes to delivering this in existing large companies, it is object oriented programming in a largely procedural programming world.