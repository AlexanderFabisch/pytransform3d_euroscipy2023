# Transformations in Three Dimensions

[Talk](https://pretalx.com/euroscipy-2023/talk/TVJEAD/)

**Session type:** Talk (15 minutes)

**Track:** Scientific Applications

**Abstract as a tweet:** Introduction to 3D transformations in Python illustrated with problems in robotics

**Category [Scientific Applications]:** Robotics & IoT

**Expected audience expertise (Domain):** none

**Expected audience expertise (Python):** some

**Talk submissions only: Would you be prepared to do a poster as fallback?** - yes

**Public link to supporting material:** --

**Project Homepage / Git:** https://github.com/dfki-ric/pytransform3d


## Abstract

*Short Description (Compact description, used in schedule or social media)
Please write between 200 and 1500 characters.*

Rigid transformation in 3D are complicated due to the multitude of different
conventions and because they often form complex graphs that are difficult to
manage. In this talk I will give a brief introduction to the topic and present
the library pytransform3d as a set of tools that can help you to tame the
complexity. Throughout the talk I will use examples from robotics (imitation
learning, collision detection, state estimation, kinematics) to motivate the
discussed features, even though presented solutions are useful beyond robotics.


## Description

*Please do NOT include any personal information. Will be published on our
website. Please write between 400 and 50000 characters.*

This talk focuses on rotation and translation, that is, rigid transformations,
in three  dimensions.
There are various representations of these. We often combine several software
components with different conventions. Furthermore, we usually combine multiple
transformations that form complex graphs of transformations, and we are often
interested in transformations that are not directly available, but can be
computed from a combination of multiple transformations. Both problems can be
handled with pytransform3d, a Python library for transformations in three
dimensions.

pytransform3d offers...

* operations for most common representations of rotation / orientation and
  translation / position
* conversions between those representations
* clear documentation of conventions
* tight coupling with matplotlib to quickly visualize (or animate)
  transformations
* the TransformManager which organizes complex chains of transformations
* the UrdfTransformManager which is able to load transformations from URDF
  files
* a matplotlib-like interface to Open3D’s visualizer to display geometries and
  transformations

I will present several features of the library in this talk and I will use
examples from robotics for illustration, for example,

* imitation learning - learning robotic motion from human demonstration
* kinematics - translation of a human hand motion to a robotic hand
* collision detection - between a robot arm and it's environment
* state estimation - estimation of a robot's location and its uncertainty

There are several pitfalls that we will discuss as well.

