---
layout: project
title: Nutcracker Design Project
description: A design of a nutcracker, with calculations and discussions of usability
technologies: n/a
image: /workspaces/sp26-portfolio-rc978-dev/assets/images/Design_diagram.png
---


![Design Diagram]({{ "/workspaces/sp26-portfolio-rc978-dev/assets/images/Design_diagram.png" | relative_url }}){: class="diagram-image"}

Find: distance_handle

Given: distance_nut = 1 inch, F_cracking = 2207.25 N, F_grip = 300 N
Sources for F_cracking and F_grip are
https://link.springer.com/article/10.1007/s10071-007-0131-2#appendices
and
https://www.sciencedirect.com/topics/engineering/grip-force
respectively.

Plan:

1. Find all the forces acting on one side of the nutcracker when the nut is about to crack
2. Assume that the nut is held in place by friction. Then the forces on the lever can all be broken down into components parallel and perpendicular to it.
3. Find the moment around the hinge of the lever. This cancels out the reaction forces acting on the lever. It also results in the moment sum equation:
 F_cracking*distance_nut = F_grip*distance_handle
 Rearranging,
 distance_handle = (F_cracking/F_grip)*distance_nut
 
 Since distance_nut = 1 inch for convenience,

 distance_handle (inches) = (F_cracking/F_grip) ~ (2207.25/300 N) = 7.36 inches

 Discussion:

 Between the calculations and the final design, some tweaks were made for better use. Firstly, the nut is moved slightly closer to the hinge in order to reduce the necessary torque to crack the nut. The length of the handles were also slightly reduced to make the design more wieldly.
 The main drawback of this design results from several abstractions made in its design. Firstly, if the design is to be interpreted literally, then there is currently no mechanism to hold the nut in place, which would make it quite difficult to use. Realistically, there would be some sort of groove or a material with significant friction at the point of placement for the nut in order to hold it in place. Secondly, the design was made without considering the weight, which would also affect usability. A manufacturer would have to find a material with both the strength to withstand the torques exerted on it and the lightness to have those torques exerted easily.

 However, these aside, the design of the nutcracker provided should prove to easily break the nut. Where the nut's breaking point was slightly overestimated, the grip strength was also significantly underestimated in order to ensure that a user could easily break the nut. While this design is currently ergonomically questionable, it is mechanically feasible.



