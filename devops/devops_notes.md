# Devops

> So you want to deploy your code?

## Historical vs Mondern practices from a high level

How would you go about doing that? How did people historically do that?

- Old vs Mondern development pipelines
- Write code -> WHAT GOES HERE -> Users use application

What was before the Cloud?

What is DevOps?

- Server farms
- Cloud providers
- Serverless

## Containerization

What does Docker bring to the table? Why does everyone use it?
Why is it a HUGE deal in the industry?

## First Principals

cgroups

- [cgroups video](https://www.youtube.com/watch?v=sK5i-N34im8)
- system resources for a process
   - limit
   - account
   - prioritize

namespaces

- isolate processes so they get their own resources namespace
- isolate
   - PIDs
   - Network
      - each can have their own IP
   - Mounting
      - each can have their own sub filesystem yet share the same parent filesystem

What is a VM?

- Hyperviser
- kvm, qemu, libvirt
- multipass

chroot

- [chroot on Wikipedia](https://en.wikipedia.org/wiki/Chroot)
- debootstrap
- change what dir `/` is at
- chroot demo
- > this is how you roll distros

What is a Runtime?

- c runtime
- js runtime
   - browser runtime
   - node runtime
- Container runtime
   - start and stop containers
   - provision resources
   - isolation

What is a Container how is it different then a VM?

- no hyperviser
- isolated processes and systems that share the same kernal

## Tooling

What is Docker/Podman (OCI)?

- [OCI](https://opencontainers.org/)

What is Docker Compose?

- Why does it exist?
- differance between `docker-compose` and `docker compose`

What is CI?

- [GitHub Actions Workflow Syntax](https://docs.github.com/en/actions/reference/workflows-and-actions/workflow-syntax)
- quick show around my different projects with ci
   - funkybooboo.github.io
   - nsegcm
   - lazycsv
   - coreutils

What is CD?

- how-to-deploy-a-dockerized-fastapi-to-cloud-providers demo

What is the Cloud?

- look around gcloud and azure
- talk about basic services and use cases
- talk about why the cloud took over

A bit on Docker Swarm/K8s

- Scaling Vertically or Horizontally

## Scalibilty

Issues that come with Scalibility

- load balencers and the stateless problem
- secrets management
- roll out
- roll back

12 factor app and why its important

- activity
- what kind of bugs would happen if you didnt follow a rule?
