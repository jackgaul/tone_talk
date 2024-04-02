---
title: Opinion Space - Opinion State
author: Jack Gaul
pubDatetime: 2024-03-28T04:06:31Z
slug: opinion-space-opinion-state
featured: false
draft: false
tags:
  - opinion space
description: Vector or embedding representation of opinion state in state space.
---

## Motivation

The goal of this post is to clarify the conceptualization for an agents opinion-state as a vector in the vector space Opinion Space.

## Intro

Hopefully you have read the Opinion Space post as this post builds heavily on that idea.
The following thoughts grew out of the question: How might we model an agent in the world?

### 1. Intelligent systems exist at a general Location in opinion space. This location is their opinion state.

For this description, we will consider a 3D surface for simplicity and for ease of visualization.

Intelligent systems will exist at a certain location on this surface. I dont believe that the state of an individual system exists at an exact point as though it were a point particle. In reality it seems more likely that these states exist in a “superposition” as a cloud surrounding a location. When a measurement is done either by a query from an outside system or a self query, the opinion is collapsed to a specific point and information is generated. This space, as mentioned in my Opinion Space blog is not discrete. An intelligent systems Opinion State, when generating an opinion, exists at a node in the Opinion Graph that overlays Opinion Space.

<div>
  <img src="/assets/opinion_space/topology_graph.png" class="sm:w-1/2 mx-auto" alt="test">
</div>

### 2. Intelligent Systems move through Opinion Space at each “collapse” from the “superposition” to a specific node in the Opinion Graph.

Movement through Opinion Space occurs whenever an intelligent system is interacting with an information source, whether that be an outside source or itself.

#### Outside Source

The most obvious driver of movement comes from a systems interaction with information sources external to itself. This isnt anything revolutionary. All interactions with media ( blogs, videos, music, podcasts, movies, etc) inject information into a system. In order to reconcile this new information (whether the system agrees with it or not) translation must occur.

#### Internal System Movement

The second source of movement is self reflection. Any time an intelligent system “thinks” it must collapse its location to a specific node and generate information from that location. This is just self-reflection and occurs whenever information is generated. For humans, the most effective method seems to be writing. This process collapses thoughts from a superpostion state into a finite representation that previously was not codified. Reflection on the representation then takes place and movement occurs. I find myself doing this all the time and can bucket the reasoning into two categories. Either I dont agree with a thought I was holding internally and didnt realize it until I brought it out into the light, or there is an error in the language encoding process and what I wrote isnt exactly what I thought but it is different in such a way that I react to it and change my location in Opinion Space.

_Side note, I think this self-reflection movement occurs any time we are generating information including when we are generating information for other systems (explaining your thoughts to a friend)._

Assume for the moment we are totally isolated from external sources of information. This self reflection process, if done iteratively, will move us along a trajectory towards a local minimum in our location in Opinion Space based on some metric of “correctness”. If a system doesnt engage in self reflection, it can be thought of as unstable. Generated information may be incoherent with other generated information. The self reflection process minimizes these inconsistencies until the intelligent system has reached a local minimum where it “orbits”, oscillates, or “settles”. In plan words, given the facts the system knows and its set of logical rules, it has reached the most “correct” location in its sub-region of the Opinion Space and Opinion Graph.

<div>
  <img src="/assets/opinion_space/surface_minimum.png" class="sm:w-1/2 mx-auto" alt="test">
</div>

### 3. Intelligent Systems that are near each other have similar Opinions. This similarity metric can be described by Euclidean distance of their vectors or sub-sections of their vectors as well as the length of the shortest path in the Opinion Path.

There isnt too much to clarify here. The difference in opinion between two locations is the euclidean distance of the vectors(total opinion difference) or sub-vectors(difference of opinion in specified dimensions). Having both is useful because if we want to just compare something like movie preferences we would only like to compare the relevant dimensions. Its possible that two systems( A and B) are vastly different on fundamental dimensions but have very similar movie tastes. While system C and B have very different movie tastes but align on pretty much everything else. In this scenario, we must use a sub-section of the Opinion State vector for difference when trying to figure out proximity as its related to movies.

The length of the shortest path is necessary because I am describing the Opinion Space explixitly with a Graph component. The euclidean distance between two points may be quite small but the trajectory between the two points may be quite large.
