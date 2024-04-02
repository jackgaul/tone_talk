---
title: Opinion Space
author: Jack Gaul
pubDatetime: 2024-03-28T09:30:31Z
slug: opinion-space
featured: false
draft: false
tags:
  - Opinion Space
  - Objective Opinion Space
  - Subjective Opinion Space
  - Opinion Dynamics
description: General description of Opinion Spaces to lay the foundation for further discussions and applications on Opinion Dynamics
---

One of my interests involves the dynamics of human’s opinions. How they change over time, how we can use mathematical objects/concepts to approximate them, and how these dynamics will play out as LLMs and Generative AI in general create the majority of content online. Though I havent heard a term yet that describes this area of study, I have come across the phrase Opinion Dynamics which I will use.

In order to even start talking about the application of LLMs in the information networks were we interact and their affects on the people in the network, I need to define a representation of a humans Opinion. This representation must live in some mathematical struture. This post is an attempt to describe such a structure.

While trying to formally write about a system that can manipulate/translate a points position in Opinion Space, I really try to consider the generalization of such a system. This severely complicates a solution and requires the introduction of new conceptions to grapple with this hypothetical system and the space in which it acts.

For clarification: when I say system, I mean anything that generates information and exposed it to a network that other systems apply semantic meaning to such as videos, photos, and text that is coherent. This application of semantic meaning to information by definition changes the receives location in Opinion Space. For almost all of history, the only system that fell under this definition was humans. Now, with Gen AI, autonomous agents must also be included.

At the core, this System begs the requirement to define a distinction between a subjective Opinion Space and an objective Opinion Space. Independently, both seem quite reasonable.

- The **subjective opinion space** exists entirely in an individuals mind(or model architecture and weights). It is the _learned_ and _approximated_ instance of the **objective opinion space.**
- The **objective opinion space** is something like the set of all facts held together in relation by the fundamental laws of logic (possibly science but not clear if we require them).

## **What is an Opinion space?**

Before I describe Subjective and Objective Opinion Space and the distinction between the two, I think it is useful to describe a general preliminary construction of Opinion Space what it means for a human(or any intelligent system) to exist at a location in Opinion Space. Who knows what dimensionality requirement is needed to accurately describe a humans opinion. It is fair to say it is quite large. The dimensionality scales with the desired granularity of opinion approximation. What I mean here is that if you want someones location in Opinion Space to account for something like their favorite chocolate bar, you will need a highly dimensional space to encode that opinion. However if you are just interested in more general opinions, you can reduce dimensionality. A great example of this is the political compass which exists in 2D [Economic Scale, Social Scale]. If you could accurately place someone in this Opinion Space, you would be able to predict how they would react to different information and potentially predict how they would move in this space when introduced to new information by studying trajectories through this space taken by previous intelligent systems.

<div>
  <img src="/assets/political_compass.png" class="sm:w-1/2 mx-auto" alt="test">
</div>

### Subjective Opinion Space

My exploration on this idea has been drawn to two building blocks that make up Opinion Space. The first being “facts” and the second being “logical relations/rules” . In relation to Subjective Opinion Space, I put both in quotations because it isnt absolutely evident to me that any instantiation of an S**ubjective** Opinion Space can have a true “fact” in the sense that the “fact” that is stored/understood is a lossy encoded observation of a fact and not the fact itself. I put “logical relations/rules” in quotations because I am not convinced of the ability of a human(or any Intelligent System) to uniformly apply logic to the entirety of their opinion space.

I mean this is two ways:

1. The inability to apply any rule correctly more than once in the same way.
2. The inability to apply any rule uniformly across the entirety of the systems Subjective Opinion Space even if they can apply a rule locally. ie Systems are capable of uniformly applying rules locally but not globally.

To give an analogy, I will use the “rule” or law of gravity. The **law** of gravity is uniform across the known universe regardless of where one observes. The effects may drastically change based on the specific state of a location but the **law** itself doesnt change and even if it did we would expect it to change in an predictable/logical way (just changing the definition of the law from the get go). I am proposing that the application of our logical rules and laws in Subjective Opinion Space are not applied in the same manner and may change at specific locations in Opinion Space in ways that are not themselves logical. Meaning a higher order logical set of rules **CANNOT** accurately describe and predict the changes in logic “logic” governing an individuals **Subjective Opinion Space**. It seems reasonable to propose that a **Subjective Opinion Space** contains sub-regions where there is logical consistency but the overlap/intersection of theses subspaces are/can be illogical. Of course this suggests entire regions of space that are simply illogical as well.

### Relation to Objective Opinion Space

A pause here at my attempt to define Opinion Space in a logical manner which I have just stated is not necessarily uniformly logical. In the same way plato discussed the relation between the real world triangle and the triangle that exists in the space of forms, the S**ubjective Opinion Space** of an individual is in a way a projection of the O**bjective Opinion Space** from the forms space **WITH ERROR/DISTORTION**.

### Objective Opinion Space

The O**bjective Opinion Space** can be talked about in a more precise way simply because we can assume perfection in both the facts encoded in the space and the logical rules that define the O**bjective Opinion Space**. So much so that even the term “Opinion Space” seems to inaccurately define it. This would almost imply that whatever “opinion” exists at any location in this space is in fact the “correct” opinion to hold. I guess I believe this. This seems like the Opinion Space of G\*d, simply meaning an Omniscient Entity capable of perfect understanding and reasoning.

### Structure

Ive played with a few ideas for the actual structure of this space and have settled on two. The first one that sticks out is some high dimensional manifold. This idea is useful because we can think of peoples Subjective Opinion Spaces as being charts. Meaning a Subjective Opinion Space is an open set of elements on the manifold projected into an open subset of n-dimensional Euclidean space. Small issue is that somewhere in this process a distortion seems to occur in the projection. The benefit of the Subjective Opinion Space being Euclidean is that we can describe locations and states as embedding vectors. The other structure can be thought of as a graph, Opinion Graph, overlayed on top of the euclidean space enforcing a discreteness to the possible positions an intelligent system may occupy. In some circumstances, one might be “between” opinions (which i would say is a valid location sometimes. Liking two candy bars equally) but in general I believe opinion changes occur in a discrete way.

<div>
  <img src="/assets/graph_vectorspace.png" class="sm:w-1/2 mx-auto" alt="test">
</div>

## Wrapup

The whole goal of this post is to introduce some concepts and terms I will later use when speaking about the actual dynamics of systems in Opinion Space. As I will continue in other posts, I hope to make it clear that thinking about the mental state of intelligent systems in this framework allows us to draw insights into how social networks and information algorithms manipulate agents, for better or for worse.
