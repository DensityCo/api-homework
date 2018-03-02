# Density API Homework Assignment


## Goal

Your goal is to create an API that can handle both historical and real-time people count requests from consumers.

## Intro

This assignment encompasses a large problem set that doesn't have the clearest boundaries, by design. Our goal is to understand your thought process, documentation style, and to get a sense of how you reason about a complex system. **Please don't spend more than 3-4 hours on this**. We'd prefer incomplete work with notes on what you focused on, where you left off, and the limitations of your solution.

If you get stuck or need more information, don't hesitate to reach out for clarity!


## Context

Density DPUs (depth processing units) are mounted above doorways. The DPU sends a request to the API when a person passes underneath (+1 when towards the DPU, -1 when walking away from the DPU).

You are provided with a CSV file of raw events from a handful of DPUs, and a floorplan indicating DPUs, doorways, and spaces.

![space diagram](https://raw.githubusercontent.com/DensityCo/api-hw/trunk/space-diagram.png)


## Assignment

Your task is to accomplish the following:

- Scaffold a database structure that includes spaces, doorways, and count data.
- Document how you would store and return real-time count for spaces.
- Document how you would store and return historical count for spaces.
- Prototype an API endpoint that yields the current count of a given space at a given point in time.
- Describe the technologies you would use in production to handle this workload at scale (100,000 DPUs).

Items to take into consideration:

- DPUs are sometimes moved from one doorway to another.
- DPUs sometimes send events out of order.
- DPUs don't always send data up in real-time. Network downtime and other events can cause delayed events.


## Deliverables

For delivery of this assignment, we'd like to see:

- Database schema / SQL file.
- Protoype Python application that includes a single endpoint for current count. Focus on prototyping database query / API implementation and don't worry about best-practices with app structure.
- Documentation on real-time and historical use-cases.
- Documentation on production technologies.


## Submission
Create a new repo using your Github account with a unique name and send us the final product (please do not fork or submit a PR to this repo).

