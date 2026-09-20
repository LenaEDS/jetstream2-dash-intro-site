What Is Jetstream2?
===================

Jetstream2 is a national research cloud funded by the National Science
Foundation, with 8 petaFLOPS of compute and 17.2 PB of storage. Its defining
characteristic is that it is a **cloud, not a batch supercomputer**: instead
of submitting jobs to a queue and waiting, you get real virtual machines
with public IP addresses that stay powered on — your analysis environment
"lives" in the cloud until you tell it to stop.

Key facts
---------

- **Five regions across the US.** Indiana University (the primary region)
  plus **TACC** in Austin, Texas; Arizona State University; Cornell
  University; and the University of Hawaiʻi.
- **Modern hardware.** AMD EPYC CPUs and NVIDIA A100 GPUs, depending on the
  region and the instance type you choose.
- **OpenStack under the hood.** Work through a simple web interface
  (Exosphere), a command-line interface, or SDKs and scripting — whatever
  fits your workflow.
- **Your university login.** You authenticate with your institutional
  credentials, so there is no separate vendor account to manage.

How it differs from a cluster
-----------------------------

On a traditional HPC system you request CPU-hours, your job runs for a
while, and then the resources go away. An interactive dashboard is the
opposite: it is a named, addressable web service that must *stay up*.
Jetstream2 gives you exactly that — persistent machines with stable
addresses — which is why it is such a good fit for the kind of work
described in the next section.
