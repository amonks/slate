# Architecture

## Goals

The gifbooth architecture has one primary design goal -- flexibility, especially through the following means:

* Code sharing
* Modularity
* Well-defined client responsibilities

We should be able to:

* Write image processes one time (bullet time, 3d, new shaders, ???) and have them work on any existing and potential clients.
* Quickly compose new clients from existing modules.
* Develop clients for environments with a wide range of capabilities: a website, a mobile app, a desktop app, or even videos sent in by MMS.
* Update one module and automatically pull the update into multiple clients.

## Clients

Users interact with Gifbooth *clients*. The clients, in turn, interact with the Gifbooth *server*. 

Gifbooth clients have the following responsibilites:

1. Displaying events (ie the current gifbooth website)
2. Capturing gifs

