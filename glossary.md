# Graftcode Glossary

This glossary keeps project and documentation terminology consistent across technical, product, and business contexts.

---

## A

### Abstraction
The process of hiding complex implementation details from developers. Graftcode provides higher-level abstraction by handling cross-runtime and cross-language communication.

### Analyzer
A technology-specific component that inspects a module or package public surface and produces a Unified Graft Model (UGM).  

### Artifact Feeds
Repositories that host software packages (for example npm, NuGet, Maven, PyPI, or private feeds such as Artifactory). Graftcode Modules can index these feeds.

---

## C

### Called Technology
The technology/runtime where the target implementation executes (receiver side).

### Calling Technology
The technology/runtime used by the consumer application (caller side) that imports and uses a generated Graft client.

### Cross-Language Collaboration
Using modules written in different languages as typed dependencies across technology boundaries.

---

## G

### Generator (Strongly Typed Interface Generator)
The primary term for components that produce strongly typed Graft clients from the Unified Graft Model (UGM) for a selected calling technology.

### Graft
An auto-generated, strongly typed client package that mirrors a module public interface and can be consumed like a native dependency.

### GraftConfig
The client-side configuration entry point exposed by generated Grafts, used to set host/runtime connection options.

### Graft Connection String
A structured configuration string used to define transport and runtime connection settings for a Graft.

### Graft Interface
The generated API surface of a Graft in the calling technology, including methods, types, signatures, and IDE type support.

### Graft Registry
A package registry endpoint used by package managers to install generated Grafts (for example free or project-scoped registry URLs backed by virtual feeds).

### Graftcode Engine
The backend generation service that receives package-manager requests, resolves metadata, generates the requested Graft from UGM, and returns/caches the package.  

### Graftcode Gateway
A native runtime host that loads runtimes/modules, discovers public interfaces, builds UGM, hosts Hypertube (and Vision), and executes calls. It is not a proxy, API gateway, or middleware traffic interceptor.  

### Graftcode Insights
A portal analytics capability focused on visibility into usage, runtime behavior, and operational metrics across connected services and gateways.

### Graftcode Modules
A discovery/search experience for finding packages across public and private artifact feeds and installing their Grafts.

### Graftcode Portal
The web experience for discovering modules/services, managing projects/workspaces, and obtaining install/configuration guidance for Grafts.

### Graftcode Vision
A runtime-based interface explorer that shows live exposed interfaces, install commands, and configuration examples for consuming services as Grafts.

### Grafting
The process of deriving UGM from exposed interfaces and generating a technology-specific Graft package for consumption.

### Grafting Agent
A legacy naming used in parts of the ecosystem for the orchestration layer that coordinates resolving, analysis, and generation workflows. In current docs, this is generally represented as the Graftcode Engine plus platform components.

---

## H

### Hypertube
The runtime bridge that executes strongly typed calls in-memory or remotely and carries invocation intent across runtimes.  

---

## I

### In-Memory Execution
Execution mode where caller and receiver runtimes run in the same process, with calls performed without network transport.

### Integration Layer
A component enabling communication between systems or modules. With Graftcode, integration is driven by generated typed clients and runtime bridging, reducing the need for hand-written API integration layers.

### Intention Invocation Protocol (IIP)
A binary protocol representing programming intent (not endpoint contracts), used by Hypertube for invocation execution across runtimes.

---

## M

### Modular Monolith
An architectural pattern where a single application is composed of well-defined independent modules. Graftcode can enable modules written in different languages to interoperate under one architecture.

---

## P

### Package Manager
A dependency tool (for example npm, NuGet, Maven, PyPI) used to install and manage Graft packages.

### Project
A scoped unit in the platform that groups services, gateways, virtual feeds, and related configuration for a specific system or environment.

---

## R

### Resolver
A component that fetches and resolves source packages/versions/dependencies from artifact repositories.

---

## S

### Service Map
A visual representation of service and gateway relationships/dependencies in the platform context.

### Strongly Typed Client
A client library with explicit method/type contracts validated by language tooling and compilation/runtime type systems.

---

## U

### Unified Graft Model (UGM)
A language-agnostic model of exposed interfaces (types, methods, signatures) used as the generation and runtime compatibility source of truth.

---

## V

### Virtual Feed
A project-scoped logical feed where exposed modules are registered and made available as versioned Grafts per package ecosystem.

---

## W

### Workspace
A top-level organizational unit in the Graftcode platform/portal that groups projects, services, and team collaboration context.

### Wrapper
A layer that exposes another module through a different interface. A Graft can be viewed as an auto-generated typed wrapper over runtime invocation.
