# Awesome Docker with stars

> A curated list of projects for Docker.

If you would like to contribute, please read [CONTRIBUTING.md](https://github.com/veggiemonk/awesome-docker/blob/master/.github/CONTRIBUTING.md) ⭐ 36,628 | 🐛 23 | 📅 2026-07-29 first.
If this list is not complete, you can contribute to make it so.
If you see a link here that is not (any longer) a good fit, you can fix it by submitting a [pull request][editreadme] to improve this file. Thank you!

**The project has to be for Docker, not just using Docker.**

> Rule of thumb: if removing the Docker integration wouldn't kill the project's value proposition, it doesn't belong in the this list.

The creators and maintainers of this list do not receive any form of payment to accept a change made by any contributor.
This page is not an official Docker product in any way.
It is a list of links to projects and is maintained by volunteers.
Everybody is welcome to contribute.
The goal of this repo is to index open-source projects, not to advertise for profit.

> Docker is an open platform for developers and sysadmins to build, ship, and run distributed applications. Consisting of Docker Engine, a portable, lightweight runtime and packaging tool, and Docker Hub, a cloud service for sharing applications and automating workflows, Docker enables apps to be quickly assembled from components and eliminates the friction between development, QA, and production environments. As a result, IT can ship faster and run the same app, unchanged, on laptops, data center VMs, and any cloud.

*Source:* [What is Docker](https://www.docker.com/why-docker/)

# Contents <!-- omit in toc -->

<!-- TOC -->

* [Projects](#projects)
  * [Engine & Runtime](#engine--runtime)
  * [Building Images](#building-images)
    * [Builder](#builder)
    * [Base Images](#base-images)
    * [Dockerfile](#dockerfile)
    * [Linter](#linter)
  * [Image Lifecycle](#image-lifecycle)
    * [Registry](#registry)
    * [Registry CLI](#registry-cli)
    * [Image Scanning & SBOM](#image-scanning--sbom)
    * [Supply Chain](#supply-chain)
  * [Running Containers](#running-containers)
    * [Composition](#composition)
    * [Orchestration](#orchestration)
    * [Deployment & Platforms](#deployment--platforms)
    * [Garbage Collection](#garbage-collection)
  * [Networking & Proxies](#networking--proxies)
    * [Networking](#networking)
    * [Reverse Proxy](#reverse-proxy)
  * [Storage & Data](#storage--data)
  * [Observability](#observability)
  * [Security](#security)
  * [User Interfaces](#user-interfaces)
    * [Desktop](#desktop)
    * [Terminal](#terminal)
    * [Web](#web)
    * [IDE Integrations](#ide-integrations)
  * [Developer Workflow](#developer-workflow)
    * [API Client](#api-client)
    * [CI/CD](#cicd)
    * [Development Environment](#development-environment)
    * [Serverless](#serverless)
    * [Testing](#testing)
    * [Wrappers](#wrappers)
  * [In-Container Tooling](#in-container-tooling)
* [Learning Resources](#learning-resources)
  * [Where to Start](#where-to-start)
  * [Where to Start (Windows)](#where-to-start-windows)
  * [Books & Tutorials](#books--tutorials)
  * [Awesome Lists](#awesome-lists)
  * [Demos and Examples](#demos-and-examples)
  * [Good Tips](#good-tips)
  * [Raspberry Pi & ARM](#raspberry-pi--arm)
  * [Security Articles](#security-articles)
  * [Videos](#videos)
  * [Communities and Meetups](#communities-and-meetups)
    * [Brazilian](#brazilian)
    * [English](#english)
    * [Russian](#russian)
    * [Spanish](#spanish)
* [Stargazers over time](#stargazers-over-time)

<!-- /TOC -->

# Projects

## Official Projects

* [Moby](https://github.com/moby/moby) ⭐ 72,014 | 🐛 3,876 | 🌐 Go | 📅 2026-08-13
* [Docker Compose](https://github.com/docker/compose/) ⭐ 38,080 | 🐛 100 | 🌐 Go | 📅 2026-08-13 - Define and run multi-container applications with Docker.
* [Docker Hub](https://hub.docker.com)
* [Docker Registry][distribution] - The Docker toolset to pack, ship, store, and deliver content

## Engine & Runtime

* [podman](https://github.com/containers/libpod) ⭐ 32,547 | 🐛 1,118 | 🌐 Go | 📅 2026-08-13 - Libpod is a library used to create container pods. Home of Podman.
* [colima](https://github.com/abiosoft/colima) ⭐ 30,347 | 🐛 385 | 🌐 Go | 📅 2026-08-08 - Container runtimes on macOS (and Linux) with minimal setup.
* [containerd](https://github.com/containerd/containerd) ⭐ 21,113 | 🐛 489 | 🌐 Go | 📅 2026-08-12 - An open and reliable container runtime.
* [gVisor](https://github.com/google/gvisor) ⭐ 19,070 | 🐛 772 | 🌐 Go | 📅 2026-08-13 - Application Kernel for Containers.
* [runc](https://github.com/opencontainers/runc) ⭐ 13,399 | 🐛 344 | 🌐 Go | 📅 2026-08-11 - CLI tool for spawning and running containers according to the OCI specification.
* [youki](https://github.com/youki-dev/youki) ⭐ 7,535 | 🐛 143 | 🌐 Rust | 📅 2026-08-12 - Container runtime written in Rust, implementing the OCI runtime specification.
* [cri-o](https://github.com/cri-o/cri-o) ⭐ 5,651 | 🐛 134 | 🌐 Go | 📅 2026-08-13 - Open Container Initiative-based implementation of Kubernetes Container Runtime Interface.
* [lxc](https://github.com/lxc/lxc) ⭐ 5,239 | 🐛 148 | 🌐 C | 📅 2026-07-23 - LXC - Linux Containers.
* [runtime-tools](https://github.com/opencontainers/runtime-tools) ⭐ 492 | 🐛 72 | 🌐 Go | 📅 2026-03-16 - Oci-runtime-tool is a collection of tools for working with the OCI runtime specification.
* [Mocker](https://github.com/us/mocker) ⭐ 321 | 🐛 1 | 🌐 Swift | 📅 2026-08-09 - Docker-compatible container CLI for macOS, built on Apple's Containerization framework.

## Building Images

### Builder

Applications designed to help or simplify building **new** images

* [DockerSlim](https://github.com/docker-slim/docker-slim) ⭐ 23,387 | 🐛 211 | 🌐 Go | 📅 2026-08-02 shrinks fat Docker images creating the smallest possible images.
* [earthly](https://github.com/earthly/earthly) ⭐ 12,047 | 🐛 743 | 🌐 Go | 📅 2025-10-23 - Containerized build automation with Dockerfile-meets-Makefile syntax.
* [BuildKit](https://github.com/moby/buildkit) ⭐ 10,186 | 🐛 918 | 🌐 Go | 📅 2026-08-13 - Concurrent, cache-efficient, and Dockerfile-agnostic builder toolkit.
* [buildah](https://github.com/containers/buildah) ⭐ 8,978 | 🐛 270 | 🌐 Go | 📅 2026-08-13 - A tool that facilitates building OCI images.
* [ko](https://github.com/ko-build/ko) ⭐ 8,491 | 🐛 54 | 🌐 Go | 📅 2026-08-13 - Build and deploy Go applications as container images without a Dockerfile.
* [buildx](https://github.com/docker/buildx) ⭐ 4,473 | 🐛 388 | 🌐 Go | 📅 2026-08-11 - Official Docker CLI plugin for multi-platform builds backed by BuildKit.
* [img](https://github.com/genuinetools/img) ⭐ 3,989 | 🐛 110 | 🌐 Go | 📅 2024-05-19 - Standalone, daemon-less, unprivileged Dockerfile and OCI compatible container image builder.
* [runlike](https://github.com/lavie/runlike) ⭐ 2,937 | 🐛 8 | 🌐 Python | 📅 2026-04-27 - Generate `docker run`command and options from running containers.
* [apko](https://github.com/chainguard-dev/apko) ⭐ 1,663 | 🐛 142 | 🌐 Go | 📅 2026-08-12 - Declarative OCI image builder from apk packages; reproducible by design.
* [Whaler](https://github.com/P3GLEG/Whaler) ⭐ 1,190 | 🐛 8 | 🌐 Go | 📅 2026-04-08 - Program to reverse Docker images into Dockerfiles.
* [nix2container](https://github.com/nlewo/nix2container) ⭐ 893 | 🐛 83 | 🌐 Go | 📅 2026-04-06 - Build OCI images with Nix without `docker load` round-trips.
* [ansible-bender](https://github.com/ansible-community/ansible-bender) ⭐ 698 | 🐛 45 | 🌐 Python | 📅 2026-01-07 - A tool utilising `ansible` and `buildah`.
* [RAUDI](https://github.com/cybersecsi/RAUDI) ⭐ 560 | 🐛 1 | 🌐 Python | 📅 2026-08-06 - A tool to automatically update (and optionally push to Docker Hub) Docker Images for 3rd party software whenever theres is a new release/update/commit.
* [HPC Container Maker](https://github.com/NVIDIA/hpc-container-maker) ⭐ 514 | 🐛 10 | 🌐 Python | 📅 2026-08-13 - Generates Dockerfiles from a high level Python recipe, including building blocks for High-Performance Computing components.
* [dlayer](https://github.com/orisano/dlayer) ⭐ 446 | 🐛 6 | 🌐 Go | 📅 2026-08-06 - Docker layer analyzer.
* [docker-repack](https://github.com/orf/docker-repack) ⭐ 167 | 🐛 7 | 🌐 Rust | 📅 2025-04-24 - Repacks a Docker image into a smaller, more efficient version that makes it significantly faster to pull.
* [cekit](https://github.com/cekit/cekit) ⭐ 113 | 🐛 31 | 🌐 Python | 📅 2026-06-22 - A tool used by openshift to build base images using different build engines.
* [docker-companion](https://github.com/mudler/docker-companion) ⭐ 47 | 🐛 5 | 🌐 Go | 📅 2025-05-28 - A command line tool written in Golang to squash and unpack docker images.
* [essex](https://github.com/utensils/essex) ⭐ 38 | 🐛 0 | 🌐 Rust | 📅 2025-03-18 - Boilerplate for Docker Based Projects: Essex is a CLI utility written in bash to quickly setup clean and consistent Docker projects with Makefile driven workflows.
* [packer](https://developer.hashicorp.com/packer/integrations/hashicorp/docker/latest/components/builder/docker) - Hashicorp tool to build machine images including docker image integrated with configuration management tools like chef, puppet, ansible.
* [Production-Ready Python Containers](https://pythonspeed.com/products/pythoncontainer/) - :yen: A template for creating production-ready Docker images for Python applications.

### Base Images

Minimal, hardened, or purpose-built container base images.

* [distroless](https://github.com/GoogleContainerTools/distroless) ⭐ 22,949 | 🐛 19 | 🌐 Starlark | 📅 2026-08-11 - Language focused docker images, minus the operating system.
* [Wolfi](https://github.com/wolfi-dev/os) ⭐ 1,265 | 🐛 83 | 🌐 Shell | 📅 2026-08-12 - Undistro Linux designed for containers; glibc-based, signed, daily SBOMs.
* [Chainguard Images](https://github.com/chainguard-images/images) ⭐ 690 | 🐛 113 | 🌐 HCL | 📅 2026-08-13 - Minimal, signed, SBOM-attested container images built on Wolfi.
* [melange](https://github.com/chainguard-dev/melange) ⭐ 620 | 🐛 257 | 🌐 Go | 📅 2026-08-10 - Build apk packages from declarative YAML for use with apko.
* [pglayers](https://github.com/pglayers/pglayers) ⭐ 145 | 🐛 2 | 🌐 Dockerfile | 📅 2026-08-12 - Pre-built PostgreSQL extensions as composable Docker layers. 50+ extensions, ready-to-use combined images (full, Azure-compatible).

### Dockerfile

* [Dockerfile Generator](https://github.com/ozankasikci/dockerfile-generator) ⭐ 185 | 🐛 0 | 🌐 Go | 📅 2022-05-23 `dfg` is both a Go library and an executable that produces valid Dockerfiles using various input channels.
* [Dockershelf](https://github.com/Dockershelf/dockershelf) ⭐ 97 | 🐛 0 | 🌐 Shell | 📅 2026-08-13 - A repository that serves as a collector for docker recipes that are universal, efficient and slim. Images are updated, tested and published daily via a Travis cron job.
* [Dofigen](https://github.com/lenra-io/dofigen) ⭐ 71 | 🐛 25 | 🌐 Rust | 📅 2026-08-03 - A Dockerfile generator using a simplified description in YAML or JSON format.
* [Trsuted Builds](https://dockerfile.github.io/) - Trusted Automated Docker Builds. Dockerfile Project maintains a central repository of Dockerfile for various popular open source software services runnable on a Docker container.

### Linter

* [Hadolint](https://github.com/hadolint/hadolint) ⭐ 12,351 | 🐛 201 | 🌐 Haskell | 📅 2026-08-10 - A Dockerfile linter that checks for best practices, common mistakes, and is also able to lint any bash written in `RUN` instructions;.
* [Dockadvisor](https://github.com/deckrun/dockadvisor) ⭐ 212 | 🐛 0 | 🌐 Go | 📅 2026-01-12 - Lightweight Dockerfile linter with 60+ rules, quality scoring, and security checks.
* [docker-image-size-limit](https://github.com/wemake-services/docker-image-size-limit) ⭐ 133 | 🐛 1 | 🌐 Python | 📅 2026-08-11 - A tool to keep an eye on your docker images size.

## Image Lifecycle

### Registry

Services to securely store your Docker images.

* [Harbor](https://github.com/goharbor/harbor) ⭐ 29,148 | 🐛 854 | 🌐 Go | 📅 2026-08-13 An open source trusted cloud native registry project that stores, signs, and scans content. Supports replication, user management, access control and activity auditing.
* [Kraken](https://github.com/uber/kraken) ⭐ 6,735 | 🐛 119 | 🌐 Go | 📅 2026-08-11 - Uber's Highly scalable P2P docker registry, capable of distributing TBs of data in seconds.
* [Dragonfly](https://github.com/dragonflyoss/Dragonfly2) ⭐ 3,296 | 🐛 29 | 🌐 Go | 📅 2026-08-13 - Provide efficient, stable and secure file distribution and image acceleration based on p2p technology.
* [NORA](https://github.com/getnora-io/nora) ⭐ 268 | 🐛 36 | 🌐 Rust | 📅 2026-08-12 - Lightweight multi-protocol artifact registry supporting Docker, Maven, npm, Cargo and PyPI in a single 32MB binary. Pull-through cache, Web UI, Prometheus metrics, RBAC auth.
* [kontain.me](https://github.com/imjasonh/kontain.me) ⭐ 245 | 🐛 25 | 🌐 Go | 📅 2026-08-09 - On-demand container image registry that builds and serves images when they are pulled.
* [Registryo](https://github.com/inmagik/registryo) ⭐ 16 | 🐛 0 | 🌐 JavaScript | 📅 2025-12-17 - UI and token based authentication server for onpremise docker registry.
* [nscr](https://github.com/jhstatewide/nscr) ⭐ 3 | 🐛 1 | 🌐 Kotlin | 📅 2025-10-27 - A light-weight, self-contained container registry that's easy to run and maintain.
* [Amazon Elastic Container Registry](https://aws.amazon.com/ecr/) - :yen: Amazon Elastic Container Registry (ECR) is a fully-managed Docker container registry that makes it easy for developers to store, manage, and deploy Docker container images.
* [Azure Container Registry](https://azure.microsoft.com/en-us/products/container-registry/#overview) - :yen: Manage a Docker private registry as a first-class Azure resource.
* [Cloudsmith](https://cloudsmith.com/product/formats/docker-registry) - :yen: A fully managed package management SaaS, with first-class support for public and private Docker registries (and many others, incl. Helm charts for the Kubernetes ecosystem). Has a generous free-tier and is also completely free for open-source.
* [Container Registry Service](https://container-registry.com/) - :yen: Harbor based Container Management Solution as a Service for teams and organizations. Free tier offers 1 GB storage for private repositories.
* [Cycle.io](https://cycle.io/) - :yen: Bare-metal container hosting.
* [DigitalOcean](https://www.digitalocean.com/products/container-registry) - :yen: DigitalOcean Container Registry.
* [Docker Hub](https://hub.docker.com/) provided by Docker Inc.
* [Docker Registry v2][distribution] - The Docker toolset to pack, ship, store, and deliver content
* [GCP Artifact Registry](https://docs.cloud.google.com/artifact-registry/docs) - :yen: Fast, private Docker image storage on Google Cloud Platform.
* [Gitea Container Registry](https://docs.gitea.com/usage/packages/container) - Integrated Docker registry in Gitea, ideal for private, small-scale image hosting.
* [GitHub Container Registry](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry) - GitHub's solution for storing and managing Docker images, with tight integration into GitHub Actions.
* [GitLab Container Registry](https://docs.gitlab.com/user/packages/container_registry/) - Registry focused on using its images in GitLab CI.
* [JFrog Artifactory](https://jfrog.com/artifactory/) - :yen: Artifact Repository Manager, can be used as private Docker Registry as well.
* [Quay.io](https://quay.io/) - :yen: Secure hosting for private Docker repositories.
* [RepoFlow](https://www.repoflow.io) - A simple and easy-to-use package management platform with Docker support alongside other formats like PyPI, Maven, npm, and Helm. Includes smart search, built-in Docker image scanning, and a great free option for both self-hosted and cloud use.
* [Sonatype Nexus Repository](https://www.sonatype.com/products/sonatype-nexus-repository) - Manage binaries and build artifacts across your software supply chain.

### Registry CLI

Daemonless command-line tools for inspecting, copying, and manipulating images in OCI/Docker registries.

* [skopeo](https://github.com/containers/skopeo) ⭐ 11,155 | 🐛 87 | 🌐 Go | 📅 2026-08-12 - Work with remote image registries: retrieve information, copy images, sign content.
* [crane](https://github.com/google/go-containerregistry/tree/main/cmd/crane) ⭐ 4,008 | 🐛 168 | 🌐 Go | 📅 2026-08-12 - Lightweight CLI to manipulate registry images, from `go-containerregistry`.
* [go-containerregistry](https://github.com/google/go-containerregistry) ⭐ 4,008 | 🐛 168 | 🌐 Go | 📅 2026-08-12 - Go library and CLI tools (`crane`, `gcrane`, `registry`) for working with container registries.
* [oras](https://github.com/oras-project/oras) ⭐ 2,382 | 🐛 74 | 🌐 Go | 📅 2026-08-11 - Push and pull arbitrary OCI artifacts to and from any OCI registry.
* [regctl](https://github.com/regclient/regclient) ⭐ 1,911 | 🐛 23 | 🌐 Go | 📅 2026-08-09 - Daemonless registry client; copy, inspect, modify, and sign OCI images.

### Image Scanning & SBOM

Image vulnerability scanners, SBOM generators, and digest pinning tools. Commercial entries marked `:yen:`.

* [Trivy](https://github.com/aquasecurity/trivy) ⭐ 37,378 | 🐛 247 | 🌐 Go | 📅 2026-08-12 - Aqua Security's open source simple and comprehensive vulnerability scanner for containers (suitable for CI).
* [Grype](https://github.com/anchore/grype) ⭐ 12,722 | 🐛 399 | 🌐 Go | 📅 2026-08-10 - A vulnerability scanner for container images, filesystems and SBOMs.
* [Clair](https://github.com/quay/clair) ⭐ 11,045 | 🐛 58 | 🌐 Go | 📅 2026-08-11 - Clair is an open source project for the static analysis of vulnerabilities in appc and docker containers.
* [Syft](https://github.com/anchore/syft) ⭐ 9,396 | 🐛 627 | 🌐 Go | 📅 2026-08-12 - CLI tool and library for generating a Software Bill of Materials (SBOM) from container images and filesystems.
* [oscap-docker](https://github.com/OpenSCAP/openscap) ⭐ 1,793 | 🐛 59 | 🌐 XSLT | 📅 2026-08-11 - OpenSCAP provides oscap-docker tool which is used to scan Docker containers and images.
* [Docker Scout](https://github.com/docker/scout-cli) ⭐ 454 | 🐛 70 | 🌐 Shell | 📅 2026-08-13 - Official Docker CLI for SBOM generation, vulnerability analysis, and policy evaluation.
* [Anchor](https://github.com/SongStitch/anchor/) ⭐ 24 | 🐛 1 | 🌐 Go | 📅 2025-01-15 - A tool to ensure reproducible builds by pinning dependencies inside your Dockerfiles.
* [BomLens](https://github.com/sktelecom/bomlens) ⭐ 16 | 🐛 2 | 🌐 Shell | 📅 2026-08-12 - Scan container images (plus source, binaries, and firmware) into CycloneDX SBOMs with vulnerability, license, and notice reports. Ships as a single Docker image with a web UI.
* [pindock](https://github.com/deadnews/pindock) ⭐ 3 | 🐛 1 | 🌐 Go | 📅 2026-07-31 - Pin and update Docker image digests in Dockerfiles and compose files.
* [Anchor Enterprise](https://anchore.com/) - :yen: Analyze images for CVE vulnerabilities and against custom security policies.

### Supply Chain

Signing, attestation, and provenance for container images.

* [cosign](https://github.com/sigstore/cosign) ⭐ 6,204 | 🐛 160 | 🌐 Go | 📅 2026-08-11 - Container signing, verification, and transparency log for OCI artifacts.
* [in-toto](https://github.com/in-toto/in-toto) ⭐ 1,027 | 🐛 58 | 🌐 Python | 📅 2026-08-05 - Framework for supply chain attestations; underpins SLSA and cosign provenance.
* [witness](https://github.com/in-toto/witness) ⭐ 544 | 🐛 77 | 🌐 Go | 📅 2026-08-10 - Generate and verify in-toto attestations across the build pipeline.
* [policy-controller](https://github.com/sigstore/policy-controller) ⭐ 178 | 🐛 90 | 🌐 Go | 📅 2026-08-11 - Kubernetes admission controller enforcing cosign signatures on container images.

## Running Containers

### Composition

* [kompose](https://github.com/kubernetes/kompose) ⭐ 10,604 | 🐛 18 | 🌐 Go | 📅 2026-06-15 - Go from Docker Compose to Kubernetes.
* [podman-compose](https://github.com/containers/podman-compose) ⭐ 6,187 | 🐛 338 | 🌐 Python | 📅 2026-08-11 - A script to run docker-compose.yml using podman.
* [Composerize](https://github.com/magicmark/composerize) ⭐ 3,758 | 🐛 11 | 🌐 JavaScript | 📅 2026-05-17 - Convert docker run commands into docker-compose files.
* [plash](https://github.com/ihucos/plash) ⭐ 382 | 🐛 9 | 🌐 C | 📅 2025-03-20 - A container run and build engine - runs inside docker.
* [ctk](https://github.com/ctk-hq/ctk) ⭐ 301 | 🐛 10 | 🌐 TypeScript | 📅 2026-02-15 - Visual composer for container based workloads.
* [Smalte](https://github.com/roquie/smalte) ⭐ 36 | 🐛 1 | 🌐 Nim | 📅 2021-12-08 – Dynamically configure applications that require static configuration in docker container.

### Orchestration

* [Kubernetes](https://github.com/kubernetes/kubernetes) ⭐ 124,482 | 🐛 2,874 | 🌐 Go | 📅 2026-08-12 - Open source orchestration system for Docker containers by Google.
* [Rancher](https://github.com/rancher/rancher) ⭐ 25,849 | 🐛 3,355 | 🌐 Go | 📅 2026-08-13 - An open source project that provides a complete platform for operating Docker in production.
* [Nomad](https://github.com/hashicorp/nomad) ⭐ 16,801 | 🐛 1,630 | 🌐 Go | 📅 2026-08-13 - Easily deploy applications at any scale. A Distributed, Highly Available, Datacenter-Aware Scheduler.
* [Mesos](https://github.com/apache/mesos) ⭐ 5,366 | 🐛 11 | 🌐 C++ | 📅 2026-05-15 - Resource/Job scheduler for containers, VM's and physical hosts.
* [docker rollout](https://github.com/Wowu/docker-rollout) ⭐ 3,309 | 🐛 8 | 🌐 Shell | 📅 2026-07-12 - Zero downtime deployment for Docker Compose services.
* [Swarm-cronjob](https://github.com/crazy-max/swarm-cronjob) ⭐ 881 | 🐛 36 | 🌐 Go | 📅 2026-08-11 - Create jobs on a time-based schedule on Swarm.
* [CloudSlang](https://github.com/CloudSlang/cloud-slang) ⭐ 242 | 🐛 111 | 🌐 Java | 📅 2026-08-11 - CloudSlang is a workflow engine to create Docker process automation.
* [Nebula](https://github.com/nebula-orchestrator) - A Docker orchestration tool designed to manage massive scale distributed clusters.

### Deployment & Platforms

Self-hosted and managed cloud platforms (PaaS/CaaS, deployment automation). Commercial entries marked `:yen:`.

* [Dokku](https://github.com/dokku/dokku) ⭐ 32,104 | 🐛 25 | 🌐 Shell | 📅 2026-08-12 - Docker powered mini-Heroku that helps you build and manage the lifecycle of applications.
* [caprover](https://github.com/caprover/caprover) ⭐ 15,127 | 🐛 177 | 🌐 TypeScript | 📅 2026-08-08 - \[Previously known as CaptainDuckDuck] Automated Scalable Webserver Package (automated Docker+nginx) - Heroku on Steroids.
* [Tsuru](https://github.com/tsuru/tsuru) ⭐ 5,304 | 🐛 17 | 🌐 Go | 📅 2026-08-12 - Tsuru is an extensible and open source Platform as a Service software.
* [werf](https://github.com/werf/werf) ⭐ 4,715 | 🐛 25 | 🌐 Go | 📅 2026-08-11 - Werf is a CI/CD tool for building Docker images efficiently and deploying them to Kubernetes using GitOps.
* [Convox Rack](https://github.com/convox/rack) ⭐ 1,890 | 🐛 25 | 🌐 Go | 📅 2026-08-12 - Convox Rack is open source PaaS built on top of expert infrastructure automation and devops best practices.
* [doco-cd](https://github.com/kimdre/doco-cd) ⭐ 1,609 | 🐛 13 | 🌐 Go | 📅 2026-08-13 - Lightweight GitOps and Continuous Deployment tool to deploy Docker Compose projects and Swarm stacks using polling and webhooks.
* [Grafeas](https://github.com/grafeas/grafeas) ⭐ 1,571 | 🐛 62 | 🌐 Go | 📅 2026-07-25 - A common API for metadata about containers, from image and build details to security vulnerabilities.
* [Exoframe](https://github.com/exoframejs/exoframe) ⭐ 1,154 | 🐛 12 | 🌐 TypeScript | 📅 2026-08-11 - A self-hosted tool that allows simple one-command deployments using Docker.
* [OpenRun](https://github.com/openrundev/openrun) ⭐ 930 | 🐛 0 | 🌐 Go | 📅 2026-08-12 - Builds, deploys, proxies, authenticates and auto-pauses web apps with Docker or Kubernetes.
* [swarm-ansible](https://github.com/LombardiDaniel/swarm-ansible?tab=readme-ov-file) ⭐ 58 | 🐛 0 | 🌐 HCL | 📅 2026-03-10 - Swarm-Ansible bootstraps a production-ready swarm cluster using ansible. Comes with tools to automate CI, help monitoring and traefik pre-configured for SSL certificates and simple-auth. Comes with a private registry and more!.
* [docker-to-iac](https://github.com/deploystackio/docker-to-iac) ⭐ 22 | 🐛 6 | 🌐 TypeScript | 📅 2026-08-10 - Translate docker run and commit into Infrastructure as Code templates for AWS, Render.com and DigitalOcean.
* [SwarmManagement](https://github.com/hansehe/SwarmManagement) ⭐ 22 | 🐛 0 | 🌐 Python | 📅 2026-05-05 - Swarm Management is a python application, installed with pip. The application makes it easy to manage a Docker Swarm by configuring a single yaml file describing which stacks to deploy, and which networks, configs or secrets to create.
* [Amazon ECS](https://aws.amazon.com/ecs/) - :yen: A management service on EC2 that supports Docker containers.
* [Appfleet](https://appfleet.com/) - :yen: Edge platform to deploy and manage containerized services globally; routes traffic to the closest location for low latency.
* [Azure AKS](https://azure.microsoft.com/en-us/products/kubernetes-service/) - :yen: Fully managed Kubernetes container orchestration service.
* [blackfish](https://gitlab.com/blackfish/blackfish) - A CoreOS VM to build swarm clusters for Dev & Production.
* [BosnD](https://gitlab.com/n0r1sk/bosnd) - BosnD, the boatswain daemon - A dynamic configuration file writer & service reloader for dynamically changing container environments.
* [Cloud 66](https://www.cloud66.com) - :yen: Full-stack hosted container management as a service.
* [Cloud Run Compose](https://docs.cloud.google.com/run/docs/deploy-run-compose) - :yen: Deploy `docker-compose.yaml` files directly to Google Cloud Run as a managed service.
* [Giant Swarm](https://www.giantswarm.io/) - :yen: Simple microservice infrastructure. Deploy your containers in seconds.
* [Google Container Engine](https://docs.cloud.google.com/kubernetes-engine/docs) - :yen: Docker containers on Google Cloud Computing powered by [Kubernetes][kubernetes].
* [Mesosphere DC/OS Platform](https://d2iq.com/products/dcos) - :yen: Integrated platform for data and containers built on Apache Mesos.
* [OpenShift][openshift] - An open source PaaS built on [Kubernetes][kubernetes] and optimized for Dockerized app development and deployment by [Red Hat](https://www.redhat.com/en)
* [Red Hat OpenShift Dedicated](https://www.redhat.com/en/technologies/cloud-computing/openshift/dedicated) - :yen: Fully-managed Red Hat® OpenShift® service on Amazon Web Services and Google Cloud.
* [Triton](https://www.joyent.com/) - :yen: Elastic container-native infrastructure.

### Garbage Collection

* [Docuum](https://github.com/stepchowfun/docuum) ⭐ 707 | 🐛 12 | 🌐 Rust | 📅 2026-08-12 - Least recently used (LRU) eviction of Docker images.
* [docker-custodian](https://github.com/Yelp/docker-custodian) ⭐ 374 | 🐛 15 | 🌐 Python | 📅 2026-08-05 - Keep docker hosts tidy.

## Networking & Proxies

### Networking

Container networking, overlay networks, DNS/service-discovery bridges.

* [netshoot](https://github.com/nicolaka/netshoot) ⭐ 10,931 | 🐛 41 | 🌐 Shell | 📅 2026-07-01 - The netshoot container has a powerful set of networking tools to help troubleshoot Docker networking issues.
* [Flannel](https://github.com/coreos/flannel/) ⭐ 9,521 | 🐛 24 | 🌐 Go | 📅 2026-08-13 - Flannel is a virtual network that gives a subnet to each host for use with container runtimes.
* [registrator](https://github.com/gliderlabs/registrator) ⭐ 4,676 | 🐛 257 | 🌐 Go | 📅 2025-05-22 - Service registry bridge for Docker.
* [Pipework](https://github.com/jpetazzo/pipework) ⭐ 4,253 | 🐛 5 | 🌐 Shell | 📅 2024-11-04 - Software-Defined Networking for Linux Containers, Pipework works with "plain" LXC containers, and with the awesome Docker.
* [docker-dns](https://github.com/bytesharky/docker-dns) ⭐ 5 | 🐛 0 | 🌐 C | 📅 2026-07-19 - Lightweight DNS forwarder for Docker containers, resolves container names with custom suffixes (e.g. `.docker`) on the host to simplify service discovery.
* [Calico][calico] - Calico is a pure layer 3 virtual network that allows containers over multiple docker-hosts to talk to each other.

### Reverse Proxy

Container-aware reverse proxies, ingress, and TLS-terminating front-ends with auto-discovery.

* [Træfɪk](https://github.com/containous/traefik) ⭐ 64,447 | 🐛 891 | 🌐 Go | 📅 2026-08-12 - Automated reverse proxy and load-balancer for Docker, Mesos, Consul, Etcd.
* [Nginx Proxy Manager](https://github.com/jc21/nginx-proxy-manager) ⭐ 33,852 | 🐛 928 | 🌐 TypeScript | 📅 2026-08-12 - A beautiful web interface for proxying web based services with SSL.
* [BunkerWeb](https://github.com/bunkerity/bunkerweb) ⭐ 10,803 | 🐛 178 | 🌐 Python | 📅 2026-08-13 - Open-source and next-gen Web Application Firewall (WAF).
* [Let's Encrypt Nginx-proxy Companion](https://github.com/nginx-proxy/docker-letsencrypt-nginx-proxy-companion) ⭐ 7,723 | 🐛 39 | 🌐 Shell | 📅 2026-08-05 - A lightweight companion container for the nginx-proxy. It allow the creation/renewal of Let's Encrypt certificates automatically.
* [caddy-docker-proxy](https://github.com/lucaslorentz/caddy-docker-proxy) ⭐ 4,616 | 🐛 46 | 🌐 Go | 📅 2026-07-27 - Caddy-based reverse proxy, configured with service or container labels.
* [OpenResty Manager](https://github.com/Safe3/openresty-manager) ⭐ 1,440 | 🐛 60 | 🌐 Go | 📅 2026-08-11 - The easiest using, powerful and beautiful OpenResty Manager(Nginx Enhanced Version), open source alternative to OpenResty Edge.
* [docker-flow-proxy](https://github.com/docker-flow/docker-flow-proxy) ⭐ 319 | 🐛 3 | 🌐 Go | 📅 2025-12-05 - Reconfigures proxy every time a new service is deployed, or when a service is scaled.
* [Swarm Router](https://github.com/flavioaiello/swarm-router) ⭐ 75 | 🐛 0 | 🌐 Dockerfile | 📅 2025-09-15 - A zero config service name based router for docker swarm mode with a fresh and more secure approach.
* [caddy-docker-upstreams](https://github.com/invzhi/caddy-docker-upstreams) ⭐ 38 | 🐛 0 | 🌐 Go | 📅 2026-07-15 - Docker upstreams module for Caddy, configured with container labels.
* [Docker Dnsmasq Updater](https://github.com/moonbuggy/docker-dnsmasq-updater) ⭐ 34 | 🐛 0 | 🌐 Python | 📅 2025-02-09 - Update a remote dnsmasq server with Docker container hostnames.
* [mesh-router](https://github.com/Yundera/mesh-router) ⭐ 13 | 🐛 0 | 🌐 TypeScript | 📅 2026-03-02 - Free domain(nsl.sh) provider for Docker containers with automatic HTTPS routing. Uses Wireguard VPN to securely route subdomain requests across networks. Ideal for self-hosted NAS and cloud deployments.
* [nginx-proxy][nginxproxy] - Automated nginx proxy for Docker containers using docker-gen.

## Storage & Data

* [Docker Volume Backup](https://github.com/offen/docker-volume-backup) ⭐ 3,948 | 🐛 26 | 🌐 Go | 📅 2026-08-11 Backup Docker volumes locally or to any S3 compatible storage.
* [REX-Ray](https://github.com/rexray/rexray) ⭐ 2,221 | 🐛 294 | 🌐 Go | 📅 2023-09-02 provides a vendor agnostic storage orchestration engine. The primary design goal is to provide persistent storage for Docker, Kubernetes, and Mesos.
* [Netshare](https://github.com/ContainX/docker-volume-netshare) ⭐ 1,141 | 🐛 99 | 🌐 Go | 📅 2021-04-12 Docker NFS, AWS EFS, Ceph & Samba/CIFS Volume Plugin.
* [Label Backup](https://github.com/resulgg/label-backup) ⭐ 24 | 🐛 2 | 🌐 Go | 📅 2025-10-27 - A lightweight, Docker-aware backup agent that automatically discovers and backs up containerized databases (PostgreSQL, MySQL, MongoDB, Redis) based on Docker labels. Supports local storage and S3-compatible destinations with flexible scheduling via cron expressions.
* [resq](https://github.com/mashb1t/resq) ⭐ 3 | 🐛 0 | 🌐 Shell | 📅 2026-05-17 - Restic-powered Docker backups for volumes, databases, and .env files, with or without stopping containers. Works with local, SSH, or any S3 compatible storage.
* [portworx](https://portworx.com) - :yen: Decentralized storage solution for persistent, shared and replicated volumes.
* [quobyte](https://www.quobyte.com/) - :yen: Fully fault-tolerant distributed file system with a docker volume driver.

## Observability

Monitor Docker hosts, containers, and the services running inside them. Self-hosted and SaaS together; commercial entries marked `:yen:`.

* [cAdvisor](https://github.com/google/cadvisor) ⭐ 19,355 | 🐛 65 | 🌐 Go | 📅 2026-07-20 - Analyzes resource usage and performance characteristics of running containers.
* [dockprom](https://github.com/stefanprodan/dockprom) ⭐ 6,574 | 🐛 21 | 📅 2026-03-06 - Docker hosts and containers monitoring with Prometheus, Grafana, cAdvisor, NodeExporter and AlertManager.
* [Autoheal](https://github.com/willfarrell/docker-autoheal) ⭐ 1,978 | 🐛 62 | 🌐 Shell | 📅 2025-09-09 - Monitor and restart unhealthy docker containers automatically.
* [Maintenant](https://github.com/kolapsis/maintenant) ⭐ 447 | 🐛 5 | 🌐 Go | 📅 2026-08-12 - Self-discovering infrastructure monitoring for Docker and Kubernetes. Auto-detects containers via labels, with endpoint monitoring, heartbeats, TLS certificates, resource metrics, update intelligence, and a built-in status page. Single binary with embedded SPA.
* [Doku](https://github.com/amerkurev/doku) ⭐ 442 | 🐛 8 | 🌐 Python | 📅 2025-12-26 - Doku is a simple web-based application that allows you to monitor Docker disk usage.
* [Drydock](https://github.com/CodesWhat/drydock) ⭐ 216 | 🐛 7 | 🌐 TypeScript | 📅 2026-08-12 - Container update monitoring with web dashboard, 23 registry providers, 20 notification triggers, and distributed agent architecture.
* [InfraCanvas](https://github.com/bytestrix/InfraCanvas) ⭐ 71 | 🐛 0 | 🌐 Go | 📅 2026-08-13 - Live visual map of containers, pods, volumes, and networks on any Linux server. Single binary, WebSocket-powered live updates.
* [Docker-Sentinel](https://github.com/Will-Luck/Docker-Sentinel) ⭐ 22 | 🐛 0 | 🌐 Go | 📅 2026-07-15 - Automated container updates with per-container policies, rollback safety, and a real-time web dashboard.
* [DockProbe](https://github.com/deep-on/dockprobe) ⭐ 20 | 🐛 1 | 🌐 Python | 📅 2026-04-11 - Lightweight Docker monitoring dashboard in a single container. Real-time metrics, 6 anomaly detection rules, Telegram alerts, and 16 automated security scans. Zero config, \~50MB RAM.
* [ADRG](https://github.com/jaldertech/adrg) ⭐ 11 | 🐛 0 | 🌐 Python | 📅 2026-03-07 - Dynamic Docker resource governor using cgroups v2 to manage system load.
* [Wiremap](https://github.com/codeofmario/wiremap) ⭐ 9 | 🐛 1 | 🌐 TypeScript | 📅 2026-05-02 - A self-hosted visual Docker network topology explorer with real-time log streaming, live stats, embedded terminal, and container inspection.
* [DLIA](https://github.com/zorak1103/dlia) ⭐ 7 | 🐛 1 | 🌐 Go | 📅 2026-08-11 - DLIA is an AI-powered Docker log monitoring agent that uses Large Language Models (LLMs) to intelligently analyze container logs, detect anomalies, and provide contextual insights over time.
* [AppDynamics](https://github.com/Appdynamics/docker-monitoring-extension) ⭐ 5 | 🐛 4 | 🌐 Java | 📅 2026-08-12 - :yen: Docker Monitoring extension gathers metrics from the Docker Remote API, either using Unix Socket or TCP.
* [docker-exporter](https://github.com/dlepaux/docker-exporter) ⭐ 3 | 🐛 2 | 🌐 Rust | 📅 2026-08-12 - Lightweight Prometheus exporter for Docker container metrics written in Rust. Correct cgroup v2 memory working set on ARM64 (Raspberry Pi 5), runs non-root with a read-only socket, \~7 MiB idle RAM.
* [Better Stack](https://betterstack.com/community/guides/scaling-docker/) - :yen: A Docker-compatible observability stack that delivers log aggregation and uptime monitoring for containerized apps.
* [Datadog](https://www.datadoghq.com/) - :yen: Full-stack monitoring service with first-class Docker, Kubernetes, and Mesos support.
* [DockProc](https://gitlab.com/n0r1sk/dockproc) - I/O monitoring for containers on processlevel.
* [Dozzle](dozzle) - Monitor container logs in real-time with a browser or mobile device.
* [Dynatrace](https://docs.dynatrace.com/docs/observe/infrastructure-observability/container-platform-monitoring) - :yen: Monitor containerized applications without installing agents or modifying your Run commands.
* [Grafana Docker Dashboard Template](https://grafana.com/grafana/dashboards/179-docker-prometheus-monitoring/) - A template for your Docker, Grafana and Prometheus stack.
* [Middleware](https://middleware.io/) - :yen: Monitor Docker hosts, containers, logs, and application performance from a unified observability platform.
* [Site24x7](https://www.site24x7.com/docker-monitoring.html) - :yen: Docker Monitoring for DevOps and IT, SaaS Pay-per-Host model.
* [Sysdig Monitor](https://www.sysdig.com/products/monitor) - :yen: Software or SaaS service that monitors, alerts, and troubleshoots containers using system calls; container-specific features for Docker and Kubernetes.

## Security

Container hardening, runtime security, policy, compliance, and forensics. Self-hosted and commercial together; commercial entries marked `:yen:`.

* [docker-bench-security](https://github.com/docker/docker-bench-security) ⭐ 9,686 | 🐛 29 | 🌐 Shell | 📅 2026-06-04 - Script that checks for dozens of common best-practices around deploying Docker containers in production.
* [Sysdig Falco](https://github.com/falcosecurity/falco) ⭐ 9,262 | 🐛 71 | 🌐 C++ | 📅 2026-08-03 - Sysdig Falco is an open source container security monitor. It can monitor application, container, host, and network activity and alert on unauthorized activity.
* [Checkov](https://github.com/bridgecrewio/checkov) ⭐ 8,934 | 🐛 160 | 🌐 Python | 📅 2026-08-11 - Static analysis for infrastructure as code manifests (Terraform, Kubernetes, Cloudformation, Helm, Dockerfile, Kustomize) find security misconfiguration and fix them.
* [Deepfence Threat Mapper](https://github.com/deepfence/ThreatMapper) ⭐ 5,310 | 🐛 144 | 🌐 TypeScript | 📅 2026-06-01 - Powerful runtime vulnerability scanner for kubernetes, virtual machines and serverless.
* [docker-socket-proxy](https://github.com/Tecnativa/docker-socket-proxy) ⭐ 2,694 | 🐛 48 | 🌐 Python | 📅 2026-07-27 - HAProxy-based fine-grained filter for the Docker API socket; widely used to expose a restricted socket to reverse proxies and homelab stacks.
* [KICS](https://github.com/checkmarx/kics) ⭐ 2,684 | 🐛 325 | 🌐 Open Policy Agent | 📅 2026-08-13 - An infrastructure-as-code scanning tool, find security vulnerabilities, compliance issues, and infrastructure misconfigurations early in the development cycle. Can be extended for additional policies.
* [container-explorer](https://github.com/google/container-explorer) ⭐ 106 | 🐛 2 | 🌐 Go | 📅 2026-08-09 - Forensic utility to explore Docker and containerd container details from mounted disk images.
* [CetusGuard](https://github.com/hectorm/cetusguard) ⭐ 89 | 🐛 2 | 🌐 Go | 📅 2026-04-01 - CetusGuard is a tool that protects the Docker daemon socket by filtering calls to its API endpoints.
* [compose-lint](https://github.com/tmatens/compose-lint) ⭐ 48 | 🐛 3 | 🌐 Python | 📅 2026-08-13 - Lints Docker Compose files for security misconfigurations — privileged containers, unpinned images, Docker socket mounts, plaintext credentials — grounded in OWASP and the CIS Docker Benchmark.
* [segspec](https://github.com/dormstern/segspec) ⭐ 16 | 🐛 0 | 🌐 Go | 📅 2026-05-06 - Extracts network dependencies from Docker Compose, Kubernetes manifests, Helm charts, and other config files to generate Kubernetes NetworkPolicies with evidence tracing.
* [Den](https://github.com/us/den) ⭐ 13 | 🐛 0 | 🌐 Go | 📅 2026-06-18 - Self-hosted sandbox runtime for AI agents with Docker containers, security hardening, REST API and WebSocket support.
* [buildcage](https://github.com/dash14/buildcage) ⭐ 10 | 🐛 1 | 🌐 TypeScript | 📅 2026-08-13 - Restricts outbound network access during Docker builds to prevent supply chain attacks, working as a drop-in BuildKit remote driver for Docker Buildx, with ready-to-use GitHub Actions.
* [Aqua Security](https://www.aquasec.com) - :yen: Securing container-based applications from Dev to Production on any platform.
* [Prisma Cloud](https://www.paloaltonetworks.com/prisma/cloud) - :yen: (Previously Twistlock Security Suite) detects vulnerabilities, hardens container images, and enforces security policies across the lifecycle of applications.
* [Sysdig Secure](https://www.sysdig.com/solutions/cloud-detection-and-response-cdr) - :yen: Sysdig Secure addresses run-time security through behavioral monitoring and defense, and provides deep forensics based on open source Sysdig for incident response.
* [Trend Micro DeepSecurity](https://www.trendmicro.com/en_us/business/products/hybrid-cloud/deep-security.html) - :yen: Trend Micro DeepSecurity offers runtime protection for container workloads and hosts as well as preruntime scanning of images to identify vulnerabilities, malware and content such as hardcoded secrets.

## User Interfaces

### Desktop

Native desktop applications for managing and monitoring docker hosts and clusters

* [Simple Docker UI](https://github.com/felixgborrego/simple-docker-ui) ⭐ 604 | 🐛 20 | 🌐 Scala | 📅 2024-09-06 - Built on Electron.
* [Stevedore](https://github.com/slonopotamus/stevedore) ⭐ 379 | 🐛 3 | 🌐 Rust | 📅 2026-07-30 - Good Docker Desktop replacement for Windows. Both Linux and Windows Containers are supported. [slonopotamus](https://github.com/slonopotamus).
* [Docker DB Manager](https://github.com/AbianS/docker-db-manager) ⭐ 165 | 🐛 10 | 🌐 TypeScript | 📅 2026-06-05 - Desktop app for managing Docker database containers with visual interface and one-click operations.
* [Docker Desktop](https://www.docker.com/products/docker-desktop/) - Official native app. Only for Windows and MacOS.

### Terminal

TUIs, CLI tools, and shell integrations for Docker.

* [dive](https://github.com/wagoodman/dive) ⭐ 54,450 | 🐛 209 | 🌐 Go | 📅 2025-12-15 - A tool for exploring each layer in a docker image.
* [lazydocker](https://github.com/jesseduffield/lazydocker) ⭐ 52,455 | 🐛 293 | 🌐 Go | 📅 2026-04-19 - The lazier way to manage everything docker. A simple terminal UI for both docker and docker-compose, written in Go with the gocui library.
* [dockly](https://github.com/lirantal/dockly) ⭐ 4,030 | 🐛 5 | 🌐 JavaScript | 📅 2026-07-23 - An interactive shell UI for managing Docker containers.
* [dry](https://github.com/moncho/dry) ⭐ 3,265 | 🐛 27 | 🌐 Go | 📅 2026-04-09 - An interactive CLI for Docker containers.
* [DockSTARTer](https://github.com/GhostWriters/DockSTARTer) ⭐ 2,570 | 🐛 4 | 🌐 Shell | 📅 2026-08-12 - DockSTARTer helps you get started with home server apps running in Docker.
* [oxker](https://github.com/mrjackwills/oxker) ⭐ 1,797 | 🐛 24 | 🌐 Rust | 📅 2026-07-24 - A simple tui to view & control docker containers.
* [lazyjournal](https://github.com/Lifailon/lazyjournal) ⭐ 1,376 | 🐛 7 | 🌐 Go | 📅 2026-08-01 - A interface for reading and filtering the logs output of Docker and Podman containers like [Dozzle](dozzle) but for the terminal with support for fuzzy find, regex and output coloring.
* [goManageDocker](https://github.com/ajayd-san/gomanagedocker) ⭐ 638 | 🐛 12 | 🌐 Go | 📅 2024-12-28 - TUI tool to view and manage your docker objects blazingly fast with sensible keybindings, also supports VIM navigation out of the box.
* [dockerfile-mode](https://github.com/spotify/dockerfile-mode) ⭐ 565 | 🐛 12 | 🌐 Emacs Lisp | 📅 2025-12-21 - An Emacs mode for handling Dockerfiles.
* [DockMate](https://github.com/shubh-io/dockmate) ⭐ 337 | 🐛 3 | 🌐 Go | 📅 2026-04-06 - Lightweight terminal-based Docker and Podman manager with a text-based user interface,.
* [dockerfilegraph](https://github.com/patrickhoefler/dockerfilegraph) ⭐ 272 | 🐛 2 | 🌐 Go | 📅 2026-07-21 - Visualize your multi-stage Dockerfiles.
* [docker pushrm](https://github.com/christian-korneck/docker-pushrm) ⭐ 152 | 🐛 6 | 🌐 Go | 📅 2024-06-10 - A Docker CLI plugin that lets you push the README.md file from the current directory to Docker Hub. Also supports Quay and Harbor.
* [decompose](https://github.com/s0rg/decompose) ⭐ 139 | 🐛 7 | 🌐 Go | 📅 2026-07-31 - Reverse-engineering tool for docker environments.
* [easydocker](https://github.com/joao-zanutto/easydocker) ⭐ 124 | 🐛 7 | 🌐 Go | 📅 2026-06-26 - A Terminal UI highly inpired by k9s levaraging beatiful BubbleTea graphics.
* [d4s](https://github.com/jr-k/d4s) ⭐ 119 | 🐛 0 | 🌐 Go | 📅 2026-07-27 - A fast, keyboard-driven terminal UI to manage Docker containers, Compose stacks, and Swarm services with the ergonomics of K9s.
* [proco](https://github.com/shiwaforce/poco) ⭐ 113 | 🐛 22 | 🌐 Python | 📅 2026-06-30 - Proco will help you to organise and manage Docker, Docker-Compose, Kubernetes projects of any complexity using simple YAML config files to shorten the route from finding your project to initialising it in your local environment.
* [scuba](https://github.com/JonathonReinhart/scuba) ⭐ 99 | 🐛 30 | 🌐 Python | 📅 2026-01-26 - Transparently use Docker containers to encapsulate software build environments,.
* [supdock](https://github.com/segersniels/supdock) ⭐ 87 | 🐛 0 | 🌐 Rust | 📅 2026-04-04 - Allows for slightly more visual usage of Docker with an interactive prompt.
* [tdocker](https://github.com/pivovarit/tdocker) ⭐ 86 | 🐛 1 | 🌐 Go | 📅 2026-08-12 - A `docker ps` replacement for everyday container operations.
* [dprs](https://github.com/durableprogramming/dprs) ⭐ 40 | 🐛 0 | 🌐 Rust | 📅 2026-07-27 - A developer-focused TUI for managing Docker containers with real-time log streaming and container management.
* [DockTUI](https://github.com/strmax195-hue/docktui) ⭐ 33 | 🐛 3 | 🌐 Python | 📅 2026-07-27 - Fast, zero-dependency terminal dashboard for Docker and Compose.
* [dctl](https://github.com/FabienD/docker-stack) ⭐ 24 | 🐛 1 | 🌐 Rust | 📅 2026-04-14 - Dctl is a Cli tool that helps developers by allowing them to execute all docker compose commands anywhere in the terminal, and more.
* [swarmcli](https://github.com/Eldara-Tech/swarmcli) ⭐ 19 | 🐛 21 | 🌐 Go | 📅 2026-08-13 - Swarm Management at the speed of thought — with real-time log streaming, instant shell access to containers, seamless port forwarding, and on-demand secret reveal capabilities, giving you full control over your Docker Swarm without breaking your flow.
* [dcinja](https://github.com/Falldog/dcinja) ⭐ 14 | 🐛 0 | 🌐 C++ | 📅 2025-06-26 - The powerful and smallest binary size of template engine for docker command line environment.
* [wharf](https://github.com/idesyatov/wharf) ⭐ 9 | 🐛 0 | 🌐 Go | 📅 2026-06-24 - A k9s-inspired TUI for Docker Compose with vim-style navigation, real-time CPU/MEM monitoring with braille charts, container file browser, SSH remote host support, and command mode.
* [docker-captain](https://github.com/lucabello/docker-captain) ⭐ 3 | 🐛 2 | 🌐 Python | 📅 2026-08-01 - A friendly CLI to manage multiple Docker Compose deployments with style — powered by Typer, Rich, questionary, and sh.
* [dockup](https://github.com/paulo-amaral/dockup) ⭐ 3 | 🐛 2 | 🌐 Go | 📅 2026-07-18 - TUI to install, harden and maintain container runtimes: Docker Engine + Compose v2, NVIDIA Container Toolkit, Podman and Apple container, with a CIS-inspired security audit.

### Web

* [Portainer](https://github.com/portainer/portainer) ⭐ 38,226 | 🐛 744 | 🌐 TypeScript | 📅 2026-08-13 - A lightweight management UI for managing your Docker hosts or Docker Swarm clusters.
* [dockge](https://github.com/louislam/dockge) ⭐ 24,049 | 🐛 164 | 🌐 TypeScript | 📅 2026-04-25 - Easy-to-use and reactive self-hosted docker compose.yaml stack-oriented manager.
* [Komodo](https://github.com/mbecker20/komodo) ⭐ 11,922 | 🐛 589 | 🌐 Rust | 📅 2026-08-11 - A tool to build and deploy software on many servers.
* [Arcane](https://github.com/getarcaneapp/arcane) ⭐ 6,965 | 🐛 126 | 🌐 Go | 📅 2026-08-13 - An easy and modern Docker management platform, built with everybody in mind.
* [Swarmpit](https://github.com/swarmpit/swarmpit) ⭐ 3,484 | 🐛 179 | 🌐 Clojure | 📅 2026-07-01 - Swarmpit provides simple and easy to use interface for your Docker Swarm cluster. You can manage your stacks, services, secrets, volumes, networks etc.
* [docker-swarm-visualizer](https://github.com/dockersamples/docker-swarm-visualizer) ⭐ 3,338 | 🐛 11 | 🌐 JavaScript | 📅 2024-10-26 - Visualizes Docker services on a Docker Swarm (for running demos).
* [Docker Registry Browser](https://github.com/klausmeyer/docker-registry-browser) ⭐ 697 | 🐛 9 | 🌐 Ruby | 📅 2026-08-11 - Web Interface for the Docker Registry HTTP API v2.
* [Container Web TTY](https://github.com/wrfly/container-web-tty) ⭐ 259 | 🐛 12 | 🌐 Go | 📅 2026-04-16 - Connect your containers via a web-tty.
* [usulnet](https://github.com/fr4nsys/usulnet) ⭐ 125 | 🐛 2 | 🌐 Go | 📅 2026-05-21 - A complete and modern Docker management platform designed for sysadmin, devops with enterprise grade tools, cve scanner, ssh, rdp on web and much more.
* [CASA](https://github.com/knrdl/casa) ⭐ 87 | 🐛 1 | 🌐 Svelte | 📅 2026-08-13 - Outsource the administration of a handful of containers to your co-workers,.

### IDE Integrations

* JetBrains IDEs (IntelliJ IDEA, GoLand, WebStorm, CLion etc.) has [built-in Docker plugin](https://www.jetbrains.com/help/idea/docker.html#managing-images)
* Eclipse [Docker Tooling plugin](https://www.eclipse.org/community/eclipse_newsletter/2016/july/article2.php)
* [docker.el](https://github.com/Silex/docker.el) ⭐ 826 | 🐛 7 | 🌐 Emacs Lisp | 📅 2026-08-03 Manage docker from Emacs.

## Developer Workflow

### API Client

* [dockerode](https://github.com/apocas/dockerode) ⭐ 4,934 | 🐛 25 | 🌐 JavaScript | 📅 2026-08-10 - Docker Remote API node.js module.
* [Docker.DotNet](https://github.com/Microsoft/Docker.DotNet) ⭐ 2,413 | 🐛 187 | 🌐 C# | 📅 2025-08-28 - C#/.NET HTTP client for the Docker remote API.
* [go-dockerclient](https://github.com/fsouza/go-dockerclient/) ⭐ 2,242 | 🐛 17 | 🌐 Go | 📅 2026-08-10 - Go HTTP client for the Docker remote API.
* [docker-maven-plugin](https://github.com/fabric8io/docker-maven-plugin) ⭐ 1,933 | 🐛 527 | 🌐 Java | 📅 2026-08-09 - A Maven plugin for running and creating Docker images.
* [sbt-docker](https://github.com/marcuslonnberg/sbt-docker) ⭐ 732 | 🐛 34 | 🌐 Scala | 📅 2024-12-12 - Create Docker images directly from sbt.
* [docker-controller-bot](https://github.com/dgongut/docker-controller-bot) ⭐ 257 | 🐛 14 | 🌐 Python | 📅 2026-07-22 - Telegram bot to control docker containers.
* [contajners](https://github.com/lispyclouds/contajners) ⭐ 150 | 🐛 0 | 🌐 Clojure | 📅 2026-08-13 - An idiomatic, data-driven, REPL friendly Clojure client for OCI container engines.
* [Docker Client for JVM](https://github.com/gesellix/docker-client) ⭐ 123 | 🐛 25 | 🌐 Groovy | 📅 2026-08-12 - A Docker remote api client library for the JVM, written in Groovy.
* [Gradle Docker plugin](https://github.com/gesellix/gradle-docker-plugin) ⭐ 82 | 🐛 12 | 🌐 Java | 📅 2026-08-12 - A Docker remote api plugin for Gradle.
* [Portainer stack utils](https://github.com/greenled/portainer-stack-utils) ⭐ 75 | 🐛 14 | 🌐 Go | 📅 2025-12-05 - Bash script to deploy/update/undeploy Docker stacks in a Portainer instance from a docker-compose yaml file.
* [Docker.Registry.DotNet](https://github.com/ChangemakerStudios/Docker.Registry.DotNet) ⭐ 43 | 🐛 6 | 🌐 C# | 📅 2025-10-06 - .NET (C#) Client Library for interacting with a Docker Registry API (v2).
* [Docker Client TypeScript](https://gitlab.com/masaeedu/docker-client) - Docker API client for JavaScript, automatically generated from Swagger API definition from moby repository.

### CI/CD

Self-hosted CI engines, build accelerators, and hosted services that target Docker workflows. Commercial entries marked `:yen:`.

* [Drone](https://github.com/drone/drone) ⭐ 37,806 | 🐛 103 | 🌐 Go | 📅 2026-08-12 - Continuous integration server built on Docker and configured using YAML files.
* [Diun](https://github.com/crazy-max/diun) ⭐ 4,842 | 🐛 98 | 🌐 Go | 📅 2026-08-11 - Receive notifications when an image or repository is updated on a Docker registry.
* [dockcheck](https://github.com/mag37/dockcheck) ⭐ 2,475 | 🐛 8 | 🌐 Shell | 📅 2026-08-11 - A script checking updates for docker images without pulling then auto-update selected/all containers. With notifications, pruning and more.
* [Captain](https://github.com/harbur/captain) ⭐ 776 | 🐛 20 | 🌐 Go | 📅 2025-05-25 - Convert your Git workflow to Docker containers ready for Continuous Delivery.
* [Docker plugin for Jenkins](https://github.com/jenkinsci/docker-plugin/) ⭐ 499 | 🐛 94 | 🌐 Java | 📅 2026-08-12 - The aim of the docker plugin is to be able to use a docker host to dynamically provision a slave, run a single build, then tear-down that slave.
* [Defang](https://github.com/DefangLabs/defang) ⭐ 163 | 🐛 214 | 🌐 Go | 📅 2026-08-12 - Deploy Docker Compose to your favorite cloud in minutes.
* [Kraken CI](https://github.com/Kraken-CI/kraken) ⭐ 160 | 🐛 96 | 🌐 Python | 📅 2026-01-15 - Modern CI/CD, open-source, on-premise system that is highly scalable and focused on testing. One of its executors is Docker. Developed.
* [Self Hosted Runner](https://github.com/youssefbrr/self-hosted-runner) ⭐ 129 | 🐛 0 | 🌐 Dockerfile | 📅 2026-07-18 - Dockerized solution for setting up a self-hosted GitHub Actions runner with support for Linux, macOS, and Windows.
* [Gantry](https://github.com/shizunge/gantry) ⭐ 90 | 🐛 0 | 🌐 Shell | 📅 2026-08-13 - Automatically update selected Docker swarm services.
* [Skipper](https://github.com/Stratoscale/skipper) ⭐ 50 | 🐛 7 | 🌐 Python | 📅 2026-07-12 - Easily dockerize your Git repository.
* [Jaypore CI](https://github.com/theSage21/jaypore_ci) ⭐ 38 | 🐛 1 | 🌐 Go | 📅 2026-03-07 - Simple, very flexible, powerful CI / CD / automation system configured in Python. Offline and local first.
* [Buddy](https://buddy.works) - :yen: The best of Git, build & deployment tools combined into one powerful tool that supercharged our development.
* [CircleCI](https://circleci.com/) - :yen: Push or pull Docker images from your build environment, or build and run containers right on CircleCI.
* [CodeFresh](https://octopus.com/codefresh) - :yen: End-to-end build, test, and share for Docker applications, with automated testing.
* [ConcourseCI](https://concourse-ci.org) - :yen: Pipeline-oriented CI SaaS platform for DevOps teams.
* [Depot](https://depot.dev) - :yen: Build Docker images fast, in the cloud. Blazing fast compute, automatic intelligent caching, and zero configuration.
* [GitLab Runner](https://gitlab.com/gitlab-org/gitlab-runner) - GitLab has integrated CI to test, build and deploy your code with the use of GitLab runners.
* [Screwdriver](https://screwdriver.cd/) - :yen: Yahoo's OpenSource buildplatform designed for Continous Delivery.
* [Semaphore CI](https://semaphore.io/) - :yen: High-performance cloud CI that builds, tests and ships containers to production.
* [Tekton CD](https://tekton.dev/) - A cloud-native pipeline resource.
* [TravisCI](https://www.travis-ci.com/) - :yen: Hosted CI for GitHub projects with Docker support.

### Development Environment

* [coder](https://github.com/coder/coder) ⭐ 14,141 | 🐛 969 | 🌐 Go | 📅 2026-08-13 - Remote development machines powered by Terraform or Docker.
* [Lando](https://github.com/lando/lando) ⭐ 4,237 | 🐛 178 | 📅 2026-08-10 - Lando is for developers who want to quickly specify and painlessly spin up the services and tools needed to develop their projects.
* [DIP](https://github.com/bibendi/dip) ⭐ 1,346 | 🐛 15 | 🌐 Ruby | 📅 2026-05-23 - CLI utility for straightforward provisioning and interacting with an application configured by docker-compose.
* [Zsh-in-Docker](https://github.com/deluan/zsh-in-docker) ⭐ 1,115 | 🐛 10 | 🌐 Shell | 📅 2024-09-30 - Install Zsh, Oh-My-Zsh and plugins inside a Docker container with one line!.
* [Gebug](https://github.com/moshebe/gebug) ⭐ 631 | 🐛 21 | 🌐 Go | 📅 2026-07-03 - A tool that makes debugging of Dockerized Go applications super easy by enabling Debugger and Hot-Reload features, seamlessly.
* [EnvCLI](https://github.com/EnvCLI/EnvCLI) ⭐ 115 | 🐛 4 | 🌐 Go | 📅 2025-06-16 - Replace your local installation of Node, Go, ... with project-specific docker containers.
* [dde](https://github.com/whatwedo/dde) ⭐ 47 | 🐛 12 | 🌐 PHP | 📅 2026-08-10 - Local development environment toolset based on Docker.
* [uniget](https://github.com/uniget-org/cli) ⭐ 24 | 🐛 17 | 🌐 Go | 📅 2026-08-11 - Uni(versal)get, the installer and updater for container tools and beyond (formerly docker-setup).
* [HarborPilot](https://github.com/potterwhite/HarborPilot) ⭐ 3 | 🐛 9 | 🌐 Shell | 📅 2026-08-04 - Automated multi-platform Docker image builder for embedded Linux development (RK3588, RV1126, RK3568). Features three-layer config inheritance, PORT\_SLOT-based port allocation, and cross-version Ubuntu support (20.04/22.04/24.04).

### Serverless

* [OpenFaaS](https://github.com/openfaas/faas) ⭐ 26,221 | 🐛 31 | 🌐 Go | 📅 2026-07-02 - A complete serverless functions framework for Docker and Kubernetes.
* [Apache OpenWhisk](https://github.com/apache/openwhisk) ⭐ 6,792 | 🐛 430 | 🌐 Scala | 📅 2026-08-11 - A serverless, open source cloud platform that executes functions in response to events at any scale.
* [Koyeb](https://www.koyeb.com/) - :yen: Koyeb is a developer-friendly serverless platform to deploy apps globally. Seamlessly run Docker containers, web apps, and APIs with git-based deployment, native autoscaling, a global edge network, and built-in service mesh and discovery.

### Testing

* [dgoss](https://github.com/goss-org/goss/tree/master/extras/dgoss) ⭐ 5,946 | 🐛 69 | 🌐 Go | 📅 2026-08-11 - A fast YAML based tool for validating docker containers.
* [Pumba](https://github.com/alexei-led/pumba) ⭐ 3,101 | 🐛 20 | 🌐 Go | 📅 2026-07-27 - Chaos testing tool for Docker. Can be deployed on kubernetes and CoreOS cluster.
* [Container Structure Test](https://github.com/GoogleContainerTools/container-structure-test) ⭐ 2,495 | 🐛 116 | 🌐 Go | 📅 2026-07-20 - A framework to validate the structure of an image by checking the outputs of commands or the contents of the filesystem.
* [Kurtosis](https://github.com/kurtosis-tech/kurtosis) ⭐ 548 | 🐛 302 | 🌐 Go | 📅 2026-08-11 - A composable build system for multi-container test environments that provides developers with: a powerful Python-like SDK for environment configuration, a compile-time validator to verify environment behavior & setup, and a runtime for environment execution, monitoring, & debugging capabilities.

### Wrappers

* [Preevy](https://github.com/livecycle/preevy) ⭐ 2,224 | 🐛 51 | 🌐 TypeScript | 📅 2026-02-06 - Preview environments for Docker and Docker Compose projects. Test your changes and get feedback from devs and non-devs (Product/Design) by deploying pull requests to the your cloud provider as part of your CI pipeline.
* [udocker](https://github.com/indigo-dc/udocker) ⭐ 1,773 | 🐛 40 | 🌐 Python | 📅 2025-08-13 - A tool to execute simple docker containers in batch or interactive systems without root privileges.
* [subuser](https://github.com/subuser-security/subuser) ⭐ 895 | 🐛 43 | 🌐 Python | 📅 2025-02-23 - Makes it easy to securely and portably run graphical desktop applications in Docker.
* [Vagrant - Docker provider](https://developer.hashicorp.com/vagrant/docs/providers/docker/basics) - Good starting point is [vagrant-docker-example](https://github.com/bubenkoff/vagrant-docker-example) ⭐ 113 | 🐛 2 | 📅 2015-10-23.
* [Hokusai](https://github.com/artsy/hokusai) ⭐ 98 | 🐛 21 | 🌐 Python | 📅 2026-06-22 - A Docker + Kubernetes CLI for application developers; used to containerize an application and to manage its lifecycle throughout development, testing, and release cycles. From [artsy](https://github.com/artsy).

## In-Container Tooling

Tools and applications that are either installed inside containers or designed to be run as a [sidecar](https://learn.microsoft.com/en-us/azure/architecture/patterns/sidecar)

* [GoSu](https://github.com/tianon/gosu) ⭐ 4,996 | 🐛 8 | 🌐 Shell | 📅 2026-06-06 - Run this specific application as this specific user and get out of the pipeline (entrypoint script tool).
* [docker-gen](https://github.com/jwilder/docker-gen) ⭐ 4,629 | 🐛 28 | 🌐 Go | 📅 2026-08-08 - Generate files from docker container meta-data.
* [Ofelia](https://github.com/mcuadros/ofelia/) ⭐ 3,959 | 🐛 142 | 🌐 Go | 📅 2026-08-09 - Ofelia is a modern and low footprint job scheduler for docker environments, built on Go. Ofelia aims to be a replacement for the old fashioned cron. Supports configuration from container labels and/or configuration files.
* [supercronic](https://github.com/aptible/supercronic) ⭐ 2,600 | 🐛 54 | 🌐 Go | 📅 2026-07-24 - Crontab-compatible job runner, designed specifically to run in containers.
* [cdebug](https://github.com/iximiuz/cdebug) ⭐ 1,664 | 🐛 18 | 🌐 Go | 📅 2026-01-18 - Swiss-army knife for debugging running containers via ephemeral sidecars; works with Docker, containerd, and Kubernetes.
* [su-exec](https://github.com/ncopa/su-exec) ⭐ 1,023 | 🐛 17 | 🌐 C | 📅 2025-10-07 - This is a simple tool that will simply execute a program with different privileges. The program will be executed directly and not run as a child, like su and sudo does, which avoids TTY and signal issues. Why reinvent gosu? This does more or less exactly the same thing as gosu but it is only 10kb instead of 1.8MB.
* [is-docker](https://github.com/sindresorhus/is-docker) ⭐ 235 | 🐛 0 | 🌐 JavaScript | 📅 2025-09-15 - Check if the process is running inside a Docker container.
* [dockerize](https://github.com/powerman/dockerize) ⭐ 194 | 🐛 4 | 🌐 Go | 📅 2026-08-03 - Utility to simplify running applications in docker containers.
* [microcheck](https://github.com/tarampampam/microcheck) ⭐ 151 | 🐛 0 | 🌐 C | 📅 2026-07-01 - Lightweight health check utilities for Docker containers (75 KB instead of 9.3 MB for httpcheck versus cURL) in pure C - http(s), port checks, and parallel execution are included.
* [ckron](https://github.com/nicomt/ckron) ⭐ 57 | 🐛 21 | 🌐 JavaScript | 📅 2026-02-15 - A cron-style job scheduler for docker,.
* [CoreOS][coreos] - Linux for Massive Server Deployments

# Learning Resources

## Where to Start

* [Docker Curriculum](https://github.com/prakhar1989/docker-curriculum) ⭐ 6,078 | 🐛 17 | 🌐 CSS | 📅 2026-08-12: A comprehensive tutorial for getting started with Docker. Teaches how to use Docker and deploy dockerized apps on AWS with Elastic Beanstalk and Elastic Container Service.
* [Setting Python Development Environment with VScode and Docker](https://github.com/RamiKrispin/vscode-python) ⭐ 952 | 🐛 4 | 🌐 Shell | 📅 2024-02-02: A step-by-step tutorial for setting up a dockerized Python development environment with VScode, Docker, and the Dev Container extension.
* [Dockerlings](https://github.com/furkan/dockerlings) ⭐ 898 | 🐛 0 | 🌐 Shell | 📅 2026-03-22: Learn docker from inside your terminal, with a modern TUI and bite sized exercises.
* [The Docker Handbook](https://docker-handbook.farhan.dev/) An open-source book that teaches you the fundamentals, best practices and some intermediate Docker functionalities. The book is hosted on [fhsinchy/the-docker-handbook](https://github.com/fhsinchy/the-docker-handbook) ⭐ 873 | 🐛 5 | 📅 2026-04-02 and the projects are hosted on [fhsinchy/docker-handbook-projects](https://github.com/fhsinchy/docker-handbook-projects) ⭐ 1,394 | 🐛 3 | 🌐 JavaScript | 📅 2026-04-02 repository.
* [Docker katas](https://github.com/eficode-academy/docker-katas) ⭐ 290 | 🐛 14 | 🌐 Dockerfile | 📅 2026-02-20 A series of labs that will take you from "Hello Docker" to deploying a containerized web application to a server.
* [Practical Guide about Docker Commands in Spanish](https://github.com/brunocascio/docker-espanol) ⭐ 263 | 🐛 1 | 🌐 Ruby | 📅 2020-07-15 This Spanish guide contains the use of basic docker commands with real life examples.
* [Learn Docker](https://github.com/dwyl/learn-docker) ⭐ 243 | 🐛 10 | 🌐 Dockerfile | 📅 2024-01-22: step-by-step tutorial and more resources (video, articles, cheat sheets)
* [Docker for beginners](https://github.com/groda/big_data/blob/master/docker_for_beginners.md) ⭐ 87 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-04-27: A tutorial for beginners who need to learn the basics of Docker—from "Hello world!" to basic interactions with containers, with simple explanations of the underlying concepts.
* [Benefits of using Docker](https://semaphore.io/blog/docker-benefits) for development and delivery, with a practical roadmap for adoption.
* [Bootstrapping Microservices](https://www.manning.com/books/bootstrapping-microservices-with-docker-kubernetes-and-terraform) - A practical and project-based guide to building applications with microservices, starts by building a Docker image for a single microservice and publishing it to a private container registry, finishes by deploying a complete microservices application to a production Kubernetes cluster.
* [Docker Documentation](https://docs.docker.com/): the official documentation.
* [Docker for novices](https://www.youtube.com/watch?v=xsjSadjKXns) An introduction to Docker for developers and testers who have never used it. (Video 1h40, recorded linux.conf.au 2019 — Christchurch, New Zealand)
* [Docker simplified in 55 seconds](https://www.youtube.com/watch?v=vP_4DlOH1G4): An animated high-level introduction to Docker. Think of it as a visual tl;dr that makes it easier to dive into more complex learning materials.
* [Docker Training](https://training.mirantis.com) - :yen:
* [Introduction à Docker](https://blog.stephane-robert.info/docs/conteneurs/moteurs-conteneurs/docker/) A dedicated section to master Docker on a French site about DevSecOps: From the basics to best practices, including optimizing, securing your containers...
* [Learn Docker (Visually)](https://pagertree.com/learn/docker/overview) - A beginner-focused high-level overview of all the major components of Docker and how they fit together. Lots of high-quality images, examples, and resources.
* [Play With Docker](https://training.play-with-docker.com/): PWD is a great way to get started with Docker from beginner to advanced users. Docker runs directly in your browser.

**Cheatsheets**

* [wsargent](https://github.com/wsargent/docker-cheat-sheet) ⭐ 22,536 | 🐛 7 | 📅 2024-12-31 (Most popular)
* [eon01](https://github.com/eon01/DockerCheatSheet) ⭐ 3,947 | 🐛 1 | 📅 2026-02-19
* [dimonomid](https://github.com/dimonomid/docker-quick-ref) ⭐ 201 | 🐛 1 | 🌐 Makefile | 📅 2021-09-26 (PDF)
* [JensPiegsa](https://github.com/JensPiegsa/docker-cheat-sheet) ⭐ 23 | 🐛 0 | 🌐 CSS | 📅 2022-03-23

## Where to Start (Windows)

* [Docker on Windows behind a firewall](https://toedter.com/2015/05/11/docker-on-windows-behind-a-firewall/)
* [Docker Reference Architecture: Modernizing Traditional .NET Framework Applications](https://docs.mirantis.com/containers/v3.0/dockeree-ref-arch/app-dev/modernize-dotnet-apps.html) - You will learn to identify the types of .NET Framework applications that are good candidates for containerization, the "lift-and-shift" approach to containerization.
* [Docker with Microsoft SQL 2016 + ASP.NET](https://blog.alexellis.io/docker-does-sql2016-aspnet/) Demonstration running ASP.NET and SQL Server workloads in Docker
* [Exploring ASP.NET Core with Docker in both Linux and Windows Containers](https://www.hanselman.com/blog/exploring-aspnet-core-with-docker-in-both-linux-and-windows-containers) Running ASP.NET Core apps in Linux and Windows containers, using [Docker for Windows][docker-for-windows]
* [Running a Legacy ASP.NET App in a Windows Container](https://blog.sixeyed.com/dockerizing-nerd-dinner-part-1-running-a-legacy-asp-net-app-in-a-windows-container/) Steps for Dockerizing a legacy ASP.NET app and running as a Windows container
* [Windows Containers and Docker: The 101](https://www.youtube.com/watch?v=N7SG2wEyQtM) - A 20-minute overview, using Docker to run PowerShell, ASP.NET Core and ASP.NET apps.
* [Windows Containers Quick Start](https://learn.microsoft.com/en-us/virtualization/windowscontainers/about/) Overview of Windows containers, drilling down to Quick Starts for Windows 10 and Windows Server 2016

***

## Books & Tutorials

* [Cloud Native Landscape](https://github.com/cncf/landscape) ⭐ 9,956 | 🐛 59 | 📅 2026-08-12
* [Docker Blog](https://www.docker.com/blog/) - Regular updates about Docker, the community and tools.
* [Docker Certification](https://intellipaat.com/docker-training-course/?US) - :yen: Will help you to will Learn Docker containerization, running Docker containers, Image creation, Dockerfile, Docker orchestration, security best practices, and more through hands-on projects and case studies and helps to clear Docker Certified Associate.
* [Docker dev bookmarks](https://www.codever.dev/search?q=docker) - Use the tag [docker](https://www.codever.dev/bookmarks/t/docker).
* [Docker in Action, Second Edition](https://www.manning.com/books/docker-in-action-second-edition)
* [Docker in Practice, Second Edition](https://www.manning.com/books/docker-in-practice-second-edition)
* [Docker packaging guide for Python](https://pythonspeed.com/docker/) - A series of detailed articles on the specifics of Docker packaging for Python.
* [Learn Docker in a Month of Lunches](https://www.manning.com/books/learn-docker-in-a-month-of-lunches)
* [Learn Docker](https://coursesity.com/blog/best-docker-tutorials/) - Learn Docker - curated list of the top online docker tutorials and courses.
* [Programming Community Curated Resources for learning Docker](https://hackr.io/tutorials/learn-docker)

## Awesome Lists

* [Awesome Selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) ⭐ 312,337 | 🐛 0 | 📅 2026-08-12 list of Free Software network services and web applications which can be hosted locally by running in a classical way (setup local web server and run applications from there) or in a Docker container.
* [Awesome Compose](https://github.com/docker/awesome-compose) ⭐ 46,071 | 🐛 415 | 🌐 HTML | 📅 2026-08-11 - Docker Compose samples.
* [Awesome Sysadmin](https://github.com/n1trux/awesome-sysadmin) ⭐ 34,890 | 🐛 0 | 📅 2026-06-20
* [ToolsOfTheTrade](https://github.com/cjbarber/ToolsOfTheTrade) ⭐ 17,145 | 🐛 16 | 📅 2026-05-16 a list of SaaS and On premise applications
* [Awesome Kubernetes](https://github.com/ramitsurana/awesome-kubernetes) ⭐ 16,049 | 🐛 77 | 🌐 Shell | 📅 2026-06-23
* [Awesome Linux Container](https://github.com/Friz-zy/awesome-linux-containers) ⭐ 2,084 | 🐛 11 | 📅 2024-04-09 more general about container than this repo.

## Demos and Examples

* [Local Docker DB](https://github.com/alexmacarthur/local-docker-db) ⭐ 299 | 🐛 3 | 🌐 Go | 📅 2024-05-04 a list of docker-compose samples for a lot of databases
* [Webstack-micro](https://github.com/ferbs/webstack-micro) ⚠️ Archived Demo web app showing how Docker Compose might be used to set up an API Gateway, centralized authentication, background workers, and WebSockets as containerized services.
* [An Annotated Docker Config for Frontend Web Development](https://nystudio107.com/blog/an-annotated-docker-config-for-frontend-web-development) A local development environment with Docker allows you to shrink-wrap the devops your project needs as config, making onboarding frictionless.

## Good Tips

* [Docker Caveats](https://docker-saigon.github.io/post/Docker-Caveats/) What You Should Know About Running Docker In Production (written 11 APRIL 2016).
* [Docker Containers on the Desktop](https://blog.jessfraz.com/post/docker-containers-on-the-desktop/)
* [Docker vs. VMs? Combining Both for Cloud Portability Nirvana](https://www.flexera.com/blog/finops/)
* [Don't Repeat Yourself with Anchors, Aliases and Extensions in Docker Compose Files](https://medium.com/@kinghuang/docker-compose-anchors-aliases-extensions-a1e4105d70bd)
* [GUI Apps with Docker](https://fabiorehm.com/blog/2014/09/11/running-gui-apps-with-docker/)

## Raspberry Pi & ARM

* [Get Docker up and running on the RaspberryPi in three steps](https://github.com/umiddelb/armhf/wiki/Get-Docker-up-and-running-on-the-RaspberryPi-%28ARMv6%29-in-three-steps) ⭐ 733 | 🐛 0 | 🌐 Shell | 📅 2016-01-28
* [Installing, running, using Docker on armhf (ARMv7) devices](https://github.com/umiddelb/armhf/wiki/Installing,-running,-using-docker-on-armhf-%28ARMv7%29-devices) ⭐ 733 | 🐛 0 | 🌐 Shell | 📅 2016-01-28
* [Docker Pirates ARMed with explosive stuff](https://blog.hypriot.com/) Huge resource on clustering, swarm, docker, pre-installed image for SD card on Raspberry Pi
* [git push docker containers to linux devices](https://www.balena.io) Modern DevOps for IoT, leveraging git and Docker.

## Security Articles

* [How CVE's are handled on Offical Docker Images](https://github.com/docker-library/official-images/issues/1448) ⭐ 6,987 | 🐛 44 | 🌐 Shell | 📅 2026-08-12
* [Docker Secure Deployment Guidelines](https://github.com/AonCyberLabs/Docker-Secure-Deployment-Guidelines) ⭐ 608 | 🐛 1 | 📅 2016-11-01
* [CVE Scanning Alpine images with Multi-stage builds in Docker 17.05](https://github.com/tomwillfixit/alpine-cvecheck) ⭐ 11 | 🐛 0 | 🌐 Shell | 📅 2017-05-07
* [Bringing new security features to Docker](https://opensource.com/business/14/9/security-for-docker)
* [Docker Security - Quick Reference](https://binarymist.io/publication/docker-security/)
* [Docker Security: Are Your Containers Tightly Secured to the Ship? SlideShare](https://www.slideshare.net/slideshow/docker-security-are-your-containers-tightly-secured-to-the-ship/43834790)
* [Lynis is an open source security auditing tool including Docker auditing](https://cisofy.com/lynis/)
* [Security Best Practices for Building Docker Images](https://linux-audit.com/tags/docker/)
* [Software Engineering Radio interview of Docker Security Team Lead (Diogo Mónica)](https://www.se-radio.net/2017/05/se-radio-episode-290-diogo-monica-on-docker-security/)
* [Ten Docker Image Security Best Practices Cheat Sheet](https://snyk.io/blog/10-docker-image-security-best-practices/)
* [Top ten most popular docker images each contain at least 30 vulnerabilities](https://snyk.io/blog/top-ten-most-popular-docker-images-each-contain-at-least-30-vulnerabilities/)
* [Tuning Docker with the newest security enhancements](https://opensource.com/business/15/3/docker-security-tuning)
* [10 best practices to containerize Node.js web applications with Docker](https://snyk.io/blog/10-best-practices-to-containerize-nodejs-web-applications-with-docker/)

## Videos

* [Deploying and scaling applications with Docker, Swarm, and a tiny bit of Python magic](https://www.youtube.com/watch?v=GpHMTR7P2Ms) (3:11:06)
* [Docker Course](https://www.youtube.com/watch?v=UZpyvK6UGFo) (Spanish)
* [Docker for Developers](https://www.youtube.com/watch?v=FdkNAjjO5yQ) (54:26)
* [Docker from scratch](https://www.youtube.com/playlist?list=PLLhEJK7fQIxD-btrjrqdEfQHbkZnQrmqE) (1:22:01)
* [Docker: How to Use Your Own Private Registry](https://www.youtube.com/watch?v=CAewZCBT4PI) (15:01)
* [Docker in Production](https://www.youtube.com/watch?v=Glk5d5WP6MI) (36:05)
* [Docker Primer to Docker Compose](https://www.youtube.com/watch?v=G-s2GXGAjTk) (1:56:45)
* [Docker Registry from scratch](https://www.youtube.com/playlist?list=PLLhEJK7fQIxAz3d4Fj3edq7UcxEhdTCBm) (44:40)
* [Docker Swarm from scratch](https://www.youtube.com/playlist?list=PLLhEJK7fQIxAY4gZd1Wl-GsLvg-e9Ap1e) (1:41:28)
* [Extending Docker with Plugins](https://vimeo.com/110835013) (15:21)
* [From Local Docker Development to Production Deployments](https://www.youtube.com/watch?v=7CZFpHUPqXw)
* [Introduction to Docker and containers](https://www.youtube.com/watch?v=ZVaRK10HBjo) (3:09:00)
* [Logging on Docker: What You Need to Know](https://vimeo.com/123341629) (51:27)
* [Performance Analysis of Docker - Jeremy Eder](https://www.youtube.com/watch?v=6f2E6PKYb0w) (1:36:58)
* [Scalable Microservices with Kubernetes](https://www.udacity.com/course/scalable-microservices-with-kubernetes--ud615) Free Udacity course
* [State of containers: a debate with CoreOS, VMware and Google](https://www.youtube.com/watch?v=IiITP3yIRd8) (27:38)

## Communities and Meetups

### Brazilian

* [Docker BR on Telegram](https://telegram.me/dockerbr)

### English

* [Docker Community](https://www.docker.com/community/)
* [Docker Events](https://www.docker.com/events/)
* [Docker Online Meetup](https://www.meetup.com/en-AU/Docker-Online-Meetup/)
* [Docker Reddit Community](https://www.reddit.com/r/docker/)

### Russian

* [Docker Russian-speaking Community](https://t.me/docker_ru)

### Spanish

* [Docker Tips](https://dockertips.com/)

## Stargazers over time

[![Stargazers over time](https://starchart.cc/veggiemonk/awesome-docker.svg?variant=adaptive)](https://starchart.cc/veggiemonk/awesome-docker)

[calico]: https://github.com/projectcalico/calico

[coreos]: https://github.com/coreos

[distribution]: https://github.com/docker/distribution

[docker-for-windows]: https://docs.docker.com/desktop/setup/install/windows-install/

[editreadme]: https://github.com/veggiemonk/awesome-docker/edit/master/README.md

[kubernetes]: https://kubernetes.io

[nginxproxy]: https://github.com/nginx-proxy/nginx-proxy

[openshift]: https://okd.io/

[sindresorhus]: https://github.com/sindresorhus/awesome

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-13._
