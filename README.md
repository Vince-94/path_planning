# Navigation Algorithms

- [Navigation Algorithms](#navigation-algorithms)
  - [Overview](#overview)
  - [Setup](#setup)
    - [Dependencies](#dependencies)
  - [Docker](#docker)
  - [Reference](#reference)


## Overview

This project contains various implementation of path planning algorithms:
- Graph-Based algorithms
  - BFS (Breadth-First Search)
  - Dijkstra
  - A*
  - D*
- Sampling-Based Algorithms
  - PRM (Probabilistic Roadmap)
  - RTT (Rapidly-Exploring Random Tree)
- Optimization-Based Algorithms
  - CHOMP (Covariant Hamiltonian Optimization for Motion Planning)
  - STOMP (Stochastic Trajectory Optimization for Motion Planning)
  - Trajectory Optimization (e.g., MPC, iLQR, CEM)
- Grid-Based Algorithms
  - Potential Fields / Artificial Forces
  - Fast Marching Methods
- Learning-Based Planning
  - Learned Heuristics for A*
  - Learning-to-Plan
  - Sampling Distribution Learning


## Setup

### Dependencies
- Eigen
    ```sh
    sudo apt install libeigen3-dev
    ```
- SDL2
    ```sh
    sudo apt install libsdl2-dev libsdl2-ttf-dev
    ```

## Docker
- Build docker image
    ```sh
    docker compose build
    ```
- Run and enter the docker container
    ```sh
    docker compose run --rm path_planning bash
    ```


## Reference

