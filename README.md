# Hedon; Heroku on Mesos

Hedon stitches together Heroku's Cedar-14 stack docker images, buildpacks, and Mesos. It's three components are:

- A Mesos framework
	- Scheduler
	- Executor
- A CLI admin tool
- A web interface

## The Mesos Framework
Provides Cedar-14 backed build-and-execute environment, a simple scheduler for long-running applications, and basic state management in the form of config vars for each deployed application.

# Requirements
- Mesos 0.23.0
- Docker on each Mesos slave

