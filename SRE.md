# SLI

SLIs can generally help engineering teams in 2 ways and should be designed with them in mind:
* quick operational responses
* long term decision making

## SLI Domains

In order of increasing proximity to user
* logs
* application
* load balancer
* dummy client
* real client instrumentation

## SLI Properties

* observability - does the strategy capture all interactions/errors
* immediacy - does the strategy give a realtime result
* richness - how complete a picture of the systems performance by component for the interaction does the strategy provide
* accuracy - how accurate is the strategy relative to the users experience
* instrumentation penalty

Observability, immediacy and accuracy generally increase as the SLI is taken closer to the user. 

Richness decreases as you get closer to the user.

## SLI Properties and SLI Design

Quick operational responses benefit a lot from observability, immediacy and accuracy but not reliably from richness.

Long-term decision making benefits particularly from richness.

When creating and SLI strateg you want a blend of the SLIs that support operational responses and long-term decision making while minimising instrumentation penalty. 
