# UnicastMessage

# Unicast Message Implementation using Vector Clocks

This repository contains Python code for implementing a unicast message communication system using vector clocks. The system allows processes to exchange messages with each other, and keeps track of events using vector clocks to ensure causal ordering of events.

## Overview

The implementation consists of two main components:

1. `server.py`: This script sets up a server that listens for incoming messages from other processes. When a message is received, it updates the vector clock accordingly.

2. `client.py`: This script allows a user to send messages to other processes. It prompts the user to enter the sender's event number, receiver's event number, and receiver's port number. It then constructs a message with the appropriate vector clock and sends it to the specified receiver.

## Usage

To use the system, follow these steps:

1. Run the `server.py` script on each process node. Specify the port number for the node when prompted.

2. When prompted, enter the process ID for the node (1/2/3) and the number of events in the process.

3. Run the `client.py` script to send messages between processes. Specify the sender's event number, receiver's event number, and receiver's port number when prompted.

## Example

Here's an example of how to use the system:

1. Run `server.py` on each process node.
2. Enter the process ID and number of events for each node.
3. Run `client.py` to send messages between processes.

## Requirements

- Python 3.x
- `pickle` module (standard library)
- `threading` module (standard library)
- `socket` module (standard library)

