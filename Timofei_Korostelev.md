# Timofei Korostelev

Senior Software Engineer (L5), ex-Google, Cloud GPU team
Greater Seattle Area

## Contact

- Phone: +1 (425) 274-5308 (Mobile)
- Email: timofei@dranik.dev
- LinkedIn: [www.linkedin.com/in/timofei-korostelev-2b27b6159](https://www.linkedin.com/in/timofei-korostelev-2b27b6159)
- GitHub: [github.com/chudsaviet](https://github.com/chudsaviet)

## Top Skills

- Distributed Systems
- GPU
- Cloud Infrastructure
- Python, C++, Rust

## Summary

US citizen. Seattle area, on-site or hybrid. Senior Software Engineer (L5) at Google Cloud until May 2026, building and running distributed systems for Google's GPU fleet. I have 15 years of software engineering experience, including large-scale distributed systems, virtual machine hypervisor level work, and data pipelines.

On the Google Cloud GPU team, I designed and built a system that runs continuously in production, verifies hundreds of thousands of AI GPUs (Nvidia H100, H200 and B200) and found GPUs with silicon defects leading to silent data corruption. The system ran isolated across multiple Google cloud clusters, and ran computationally expensive tests on idle machines, with reserve capacity sized statistically to keep the cloud's SLA. I operated it, handled incidents and created extensive postmortems.

Before that, I worked on GPU virtualization: I wrote a C++ hypervisor module that talked to the GPU over MMIO, protected the on-GPU SPI flash chip holding the firmware, and gave the Nvidia driver (which can be compromised in a guest OS) a controlled way to reach it. This module was fully developed, but never reached large scale production because Nvidia switched from running logic in the driver to on-GPU coprocessor (GSP).

After Google, I'm building Filmtwin, a physically based simulation of film down to individual silver halide crystals, written in C++ with CUDA and OptiX.

My strengths are strong physics education, GPU fleet automation in Python, systems programming in C/C++, working knowledge of Rust, and diagnosing problems that cross hardware, hypervisor, guest operating system and driver boundaries at cloud scale. I hold a Master's degree in Applied Mathematics and Physics from MIPT, specializing in Parallel Computing.

## Experience

### Developer

*June 2026 - Present*
Seattle, Washington, United States

Designing and implementing Filmtwin, a physically based simulation of photographic film, with optimized C++ Nvidia CUDA kernels and OptiX raytracing.

Digging into modern AI.

Preparing for post-COVID software interviews.

### Google - Senior Software Engineer, GPU systems, L5

*May 2022 - May 2026 (4 years 1 month)*
Seattle, Washington, United States

Developed and operated large scale distributed systems and services made with Google's Borg and Python, and Google's low-level C++ virtual machine hypervisor.

**2025-2026, Cloud GPU team**

Sole designer and developer (with design and code reviewed by the team) of a distributed system that verifies the hardware of all Google's Nvidia H100, H200 and B200 GPUs: hundreds of thousands of devices across several cloud regions.

- Found GPUs with silicon defects causing silent data corruption.
- The system runs Nvidia's hardware correctness tests on idle machines, taking each one out of the available pool for the duration of its scan.
- Main design challenge: maximizing scan rate while always keeping enough free GPU machines in reserve for the cloud to meet its SLA.
- Reserve capacity was calculated statistically given size of fungible machines group, probability of any machine being non-operational due to a failure, and target probability of being able to find a replacement machine if one customer machine fails.
- Partitioned the system by Google clusters, so that a failure stays inside one and does not affect the whole GPU fleet.
- Built on Borg and Python, released through slow staged rollouts.
- Ran it in production: coordinated with other teams, handled incidents, wrote postmortems and fixed the root causes.

**2022-2024, Cloud GPU virtualization team**

- Supported hyperscale fleet of GPUs of all performance levels, from Nvidia T4 to Nvidia H200.
- Onboarded new GPU types into cloud.
- Developed a C++ module for Google's virtual machine hypervisor. The module interacted with GPUs using MMIO hardware interface, accessed internal SPI bus and protected access to the on-GPU SPI flash chip, which contains the firmware. This module was fully developed, but never reached large scale production because Nvidia switched from running logic in the driver to on-GPU coprocessor (GSP).

### Gap
*June 2021 - April 2022*

Preparation for software interviews.

### EPAM Systems

*6 years 2 months*

**Senior Software Engineer**
*July 2017 - May 2021 (3 years 11 months)*
Seattle metropolitan area, Washington, United States

Contract data engineering for Google, Expedia, Hotels.com and Nordstrom. Large-scale data processing on Hadoop, Hive and Spark (Scala) in AWS. Airflow scheduling, and leading offshore engineers at Expedia.

**Software Engineer**
*April 2015 - June 2017 (2 years 3 months)*
Minsk, Belarus

Offshore data engineering for Expedia Inc.

### GlowByte Consulting - Data Engineer

*October 2010 - April 2015 (4 years 7 months)*
Moscow, Russia

Data engineering.

## Education

**Moscow Institute of Physics and Technology (State University) (MIPT)**
2006-2012

Bachelor's and Master's degrees. Parallel computing. Applied physics and mathematics.