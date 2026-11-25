# PocketVE
## Development Progress 01

**Date:** November 25, 2026  
**Status:** Planning and technical preparation



## Overview

PocketVE is the public evolution of the existing Proxmox 3DS application.
The objective is to develop a standalone Proxmox VE client for Nintendo 3DS, allowing users to connect directly to their own Proxmox infrastructure.
The project is designed to go beyond basic server monitoring, with the long-term goal of providing VM and container management, terminal access and VM console viewing.



## Current Progress

The project is currently in its design and preparation phase.
The main architecture and technical direction have been defined, including direct communication with the Proxmox API, authentication, TLS security and the separation between network processing and the user interface.
The existing application is being used as the starting point for the next development stage. The public version will have its own application structure and installation process.
No public PocketVE build has been released yet.



## Test Environment

Initial testing is planned around a Proxmox VE 9.2.32 installation with:
- 6 vCPU
- 8 GB RAM
- One Proxmox node
- Local and local-lvm storage

A second nested Proxmox instance is also planned to create a two-node cluster for future migration and cluster management tests.



## Technical Priorities

The first priority is to investigate the responsiveness of the existing application.
The planned work includes measuring TLS connection times, API response times and network performance on an actual Old Nintendo 3DS.
The new architecture will focus on persistent HTTPS connections and reducing unnecessary API requests.
A QR-based server configuration system is also planned to simplify the initial setup.

## Planned Features

The intended application will include:

- Proxmox dashboard and resource monitoring.
- VM and container management.
- VM and container creation.
- Storage and task monitoring.
- Terminal access.
- VNC console viewing.
- Multiple server profiles.
- QR-based configuration.
- Native `.3dsx` and `.cia` distribution.

These features are part of the planned scope and have not yet been confirmed as implemented.



## Next Steps

The immediate development priorities are:

1. Complete the initial performance benchmarks.
2. Continue development from the existing application.
3. Implement the QR configuration workflow.
4. Prepare the independent PocketVE application structure.
5. Establish direct communication with the Proxmox API.
6. Build and test the first functional version on real 3DS hardware.




## Development Goal

The main challenge is to make a Proxmox management client genuinely usable on the original Nintendo 3DS hardware.

Performance, memory usage, network stability and usability will guide the development decisions.

There is currently no release date. The priority is to get the foundations working before expanding the application.

---

Maintained by NineToFiveNines.
