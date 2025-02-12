# nRF Connect SDK Intermediate

Notes and code related to taking the course [nRF Connect SDK Intermediate](https://academy.nordicsemi.com/courses/nrf-connect-sdk-intermediate/).

## Lesson 1 - Zephyr RTOS Thread Management

### Content

This lessons covers thread management and how to pass data between threads when using nRF Connect/Zephyr. There are two different execution contexts:

1. Thread context
2. Interrupt context

Each associated with different usage and implications.

Will cover:execution primitives, How threads ands interrupt handling co-exist. Then follows info on the life cycle of a thread and the scheduler. Finally comes the topic of exchanging data between threads.

Will be able to schedule application tasks and pass data between threads after taking this lesson. 

### Learning Objectives

- Execution variants, along with their determinism and preemption nature.
- The thread life cycle.
- Zephyr kernel options and scheduler.
- Implications of adding subsystems and networks stacks to a application.
- Application task scheduling using execution primitives and correct priority levels.
- How to pass data using messages and FIFO's.
