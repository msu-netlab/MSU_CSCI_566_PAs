# CSCI 566 - Final Project

## Instructions

Complete the following assignment in your project group.
Submit your work on D2L into the "Final Project" group submission folder.


## Learning Objectives

In this programming assignment you will:

  - Integrate the knowledge from the course on how to design and implement augmented reality (AR) communication backends


## Overview

In this final assignment you will have multiple options of what type of project to submit.
Please discuss within your group an select __one__ of the projects below.
Be sure to pay attention to the submission requirements for each type project.
If you are interested in pursuing a project not on the list, please talk with me first.



## Project Options


### A. Analysis of shared state exchange options for AR

Communication paradigms such as sockets, message queues, pub/subs, real-time databases, and blockchains, provide different tradeoffs in terms of performance and features.
Given the number of options for exchanging shared state within an augmented realidy (AR) application it is not clear which one(s) best meets application requirements.

Analyze the communication tools covered in the course and propose a set of them integrated into a shared state exchange solution that would best meet the needs of the Grenades application.
When constructing your argument consider both the features provided by the different communication paradigms as well as their performance as measured in the class.
Your ultimate task is to create a convincing argument for why the set of messaging technologies you propose for Grenades is the best option.

#### What to submit?

Submit a paper in PDF with your argument.
I will be looking for a correctly framed research problem, with your argument for the set of best technologies to use as the Technical Solution.


### B. Implementation of "Grenades"

Understanding the tradeoffs between communication technologies is step one.
An implementation of a working AR prototype would be step two.

Choose one communication technology discussed in class and use it to implement the Grenades application.
The front-end for you application can be a terminal, or a browser-based application - you do not have to implement a mobile app, or an AR program.


#### What to submit?

Submit a YouTube demo of your application with a link to your code repository in the comments.

Your demo should include a message diagram showing the different interactions between clients (servers) within your application, an illustration of the gameplay (and any other in-game functions, such as checking the score), and an analysis of the delay experienced by different types of in-game messages/actions.


### C. NoSQL front-end and back-end schemas for flexible schema migration

Distributed application implementations often separate clients from the database using an API.
The advantage of that approach is that the back-end code and the database structure may evolve independently from the client code as long as the API continues to provide transparency.
The downside is that developers need to maintain both the client code and the API that translates the client requests to database queries.
Many applications that use NoSQL databases remove the API layer to allow clients to change the shared database structures directly.
While that approach reduces the implementation effort, it makes it difficult to evolve data structure without modifying the clients.

Implement a resolution to this tradeoff by building a solution based on a front-end and back-end database schema.
The front-end databases should be directly accessible by clients using different versions of the application code.
The back-end database should collect data from the various front-end database versions and populate them with the result of new writes.

#### What to submit?

Submit a YouTube demo of your application with a link to your code repository in the comments.

Your demo should clearly state the research problem you are solving.
It should also include a demonstration of your system including examples of front-end and of back-end schema migrations.


### D. Implementation of broadcast within Pulsar

AR applications often need to efficiently broadcast data to a set of connected devices.
The support for broadcast varies between publish/subscribe solutions.
While Apache Pulsar does not implement broadcast out of the box, it does allow the definition of functions which may be called to transform data along the subscription flows.

Explore the possibility of implementing the a broadcast functionality using Pulsar functions.

#### What to Submit

Submit a YouTube demo of your application with a link to your code repository in the comments.
Alternatively, if an implementation is not possible, submit a PDF paper explaining the methods tried and the limitations of Pulsar functions in implementing broadcast.
