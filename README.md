# UAV-Assisted-Cellular-Connectivity-for-On-Ground-Devices

Our project focuses on algorithms to minimize the number of required UAVs while maximizing ground coverage and connection stability. The key algorithms we evaluated are K-means clustering, particle swarm optimization, successive convex approximation, and a hybrid K-means with particle swarm optimization.

We model the environment as a 3D space with ground users distributed in a 2D area below. Each user has a defined quality of service requirement in terms of signal-to-noise ratio. The UAVs act as aerial base stations with a constrained coverage capacity each.

The problem is formulated as a mixed integer geometric disk cover optimization to minimize UAVs required while covering all users and meeting their QoS needs. This is an NP-hard problem.

To make it tractable, we break it down into UAV placement and trajectory optimization stages. K-means clustering is applied to partition users into groups corresponding to UAV coverage zones. The smallest enclosing circle method positions UAVs over clusters.

For trajectory optimization, successive convex approximation iteratively linearizes the non-convex mobility power constraints to generate flyable paths.

Key factors in our evaluation are area coverage percentage, energy efficiency, and connection stability.

Our simulation results highlight the strengths of each algorithm. K-means clustering is efficient for distributed user placement. Successive convex approximation yields smooth flyable paths that sustain connections. The hybrid K-means particle swarm optimization strikes a balance across priority parameters.

In conclusion, this project provides an extensive evaluation of UAV base station placement and trajectory optimization algorithms tailored to environments with different coverage, energy, and reliability priorities. The findings contribute useful guidelines and performance trade-offs for selecting suitable algorithms when implementing emerging UAV-assisted communication networks.
