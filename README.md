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

### Boot-up Sequence and Execution Context

Will learn how to schedule application tasks. But first we investigate the setup for what we get ready-made when basing our application on the nRF Connect SDK.

#### Boot-up Sequence

##### Part 1: Early Boot Sequence

Initially there is a stage where the system is brought up to the point where it it is capable of executing C code, this is not covered by this course.

##### Part 2: Kernel Initialization

Second stage is the kernel initialization where static devices are enabled in two steps; `PRE_KERNEL_1` and `PRE_KERNEL_2`. Exactly what devices depends on the project setup but a Clock Control driver will always be enabled in `PRE_KERNEL_1`, and also a System Time driver in `PRE_KERNEL_1`.

##### Part 3: Multithreading Preparation

TODO