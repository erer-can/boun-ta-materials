# CMPE 250 — Data Structures & Algorithms

**Project 3 (Fall 2025): MatrixNet — The Operator's Console**

## About

MatrixNet is a *Matrix*-themed simulation engine for designing, analyzing, and hardening a covert network of "hosts" (access points, each with a clearance level) connected by "backdoor tunnels" (bidirectional edges, each with latency, bandwidth, and a firewall security level). Under the theming, it's a graph engine: hosts are vertices, tunnels are weighted edges, and the constraints (bandwidth, security, latency) turn ordinary graph queries into multi-criteria routing and analysis problems.

## What students were asked to do

Implement a system that can create and remove hosts and tunnels; compute optimal covert routes between hosts subject to bandwidth, security, and latency constraints (with ties broken by lexicographically smallest host sequence); detect compromised tunnels and critical vulnerabilities that would fragment the network (i.e., cut vertices/bridges and connectivity analysis); and generate topology reports summarizing the network's shape, statistics, and weak points. All operations needed to scale efficiently to large systems, and edge cases (missing hosts/tunnels) had to be handled explicitly. Input/output is driven through a console instruction file processed command by command.

## Context

This is a core Data Structures & Algorithms project centered on graph algorithms — shortest-path/constrained routing, connectivity, and articulation point/bridge detection — with an emphasis on both correctness and efficiency on large graphs.
