# nRF Connect SDK Intermediate

Notes and code related to taking the course [nRF Connect SDK Intermediate](https://academy.nordicsemi.com/courses/nrf-connect-sdk-intermediate/).

## Lesson 1 - Zephyr RTOS Thread Management

### Content

This lessons covers thread management and how to pass data between threads when using nRF Connect/Zephyr.

There are two different execution contexts; thread context, and interrupt context, each associated with different usage and implications.

Will also cover execution primitives, and how threads ands interrupt handling co-exist. Then follows info on the life cycle of a thread, and the scheduler. Finally comes the topic of exchanging data between threads.

We will be able to schedule application tasks and pass data between threads after taking this lesson. 

### Learning Objectives

- Execution variants, with their determinism and preemption nature.
- The thread life cycle.
- Zephyr kernel options and scheduler.
- Implications of adding subsystems and networks stacks to a application.
- Task scheduling, execution primitives, and priority levels.
- Passing data using messages and FIFO's.
