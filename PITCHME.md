# Collaboration in Open-Source Robotics

---

## MRPT

C++ framework for robotics - provide portable, well tested robotics libraries,
applications

* Hardware drivers
* Vision algorithms
* Obstacle avoidance / navigation algorithms
* Localisation/SLAM algorithms


Link: https://mrpt.org

Note: Drivers for robotics hardware - cameras or algorithms in
navigation/slam/planning

---

## GSoC Summit 2018 - Open-Source Robotics session

---?image=assets/robotic_session_orgs.png&size=contain

Note: mention what each org does
Same functionality - different levels of difficulty - specializes in a different field

---

## Actions

- Code blocks/algorithms to reuse - benchmark implementations
- Well-defined well-tested modular C++ code blocks/algorithms
- C++20 concepts for common robotics datatypes

Note:
Opportunity to understand that we do similar
Say what a concept is

---

## Robotics C++ concepts - Why

- Every project has a `Pose` class
- Non-modular code
- Newbie-hostile

Note: describe what a pose is
You have to reread the exact implementation if you want to use it -
  similar but not same interface between the different Pose classes
If you choose a Pose implementation you have to stick to that - provide
    conversion methods from/to that Pose
If you just moved in from another project/org you have to reread the
  project-specific pose interface to get the picture

---

## Robotics C++ concepts - Vision

- Community accepted `Pose` concept
- Pass *any* specific Pose by using the corresponding concept
- Benchmark the implementations
- Generic wrappers for families of algorithms

Links:

* https://github.com/MRPT/mrpt/issues/846
* https://github.com/MRPT/rfcs/tree/master/concepts
* https://github.com/bergercookie/concepts
