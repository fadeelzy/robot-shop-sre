# SRE Charter — Robot Shop

## Our mission
We exist to make reliability a feature, not an afterthought.
We own the reliability of production, share it with developers, and eliminate toil.

## Services we own
- catalogue
 user
 cart
 payment
 shipping
 ratings
 dispatch
 web

## Reliability targets (initial — will be refined on Day 14)
- Checkout flow (catalogue → cart → payment): 99.9% availability
- User login: 99.5% availability
- Product browsing: 99.5% availability

## Toil we have already identified
Technology	Typical Behavior
Nginx	         low memory, efficient
Java	         high memory
Go	         tiny footprint
Redis	         memory-sensitive
MongoDB	         RAM-heavy
MySQL	         disk-heavy
RabbitMQ	 queue/memory-sensitive
Node.js	         moderate lightweight

Highest Memory Usage  - shipping service
Highest CPU           - web Nginx
Highest Disk Activity - MySQL

2. [fill in from the README e.g. manual load-gen steps]

## On-call rotation
- Team size: [3]
- Schedule: weekly rotation
- Escalation: [Fadilah-Abdulkadir-Mahmud]

## What we won't do
- We will not accept manual deployments as the norm
- We will not accept alert fatigue
- We will not accept undocumented runbooks
