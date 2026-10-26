# KubeGuardian

KubeGuardian is a Go-based Kubernetes diagnostics tool designed to identify common workload failures, analyze Kubernetes resource states, and generate evidence-based troubleshooting reports.

The goal is to simplify the initial investigation of Kubernetes issues by bringing resource inspection, failure detection, and diagnostic recommendations into one command-line tool.

## Project Goals

- Connect to Kubernetes clusters using the Kubernetes Go client.
- Inspect pods, deployments, and Kubernetes events.
- Detect common workload failures, including `CrashLoopBackOff`, `ImagePullBackOff`, repeated container restarts, and unavailable deployment replicas.
- Generate diagnostic reports based on Kubernetes resource states and events.
- Provide actionable troubleshooting recommendations.
- Build a foundation for future continuous monitoring, alerting, and incident tracking.

## Technology Stack

- **Language:** Go
- **Container Orchestration:** Kubernetes
- **Kubernetes Integration:** Kubernetes Go Client (`client-go`)
- **Development Environment:** Windows, PowerShell, and VS Code

Additional technologies may be introduced as the project develops.

## Development Roadmap

### Phase 1 — Core Diagnostics
- [ ] Initialize the Go project and CLI.
- [ ] Connect to a local Kubernetes cluster.
- [ ] Scan pods and inspect container states.
- [ ] Detect common pod failures.
- [ ] Retrieve relevant Kubernetes events.
- [ ] Inspect deployment health.
- [ ] Generate diagnostic reports.
- [ ] Test against intentionally created Kubernetes failures.

### Future Phases
- Continuous monitoring and event-driven detection.
- Concurrent processing and work queues.
- Incident history and persistence.
- Alerts, metrics, and structured logging.
- Containerized deployment and Kubernetes integration.
- Carefully controlled remediation capabilities.

## Project Status

**In development.** The initial focus is on building and testing the core diagnostic engine against a local Kubernetes cluster.

Features will be marked as complete as they are implemented and verified.

## Getting Started

Prerequisites:
- Go
- `kubectl`
- A running Kubernetes cluster
- Access to the cluster through a valid Kubernetes configuration

Clone the repository:

```bash
git clone <your-repository-url>
cd kubeguardian
```

Run the application from the project root:

```bash
go run ./cmd/kubeguardian
```

The available commands will expand as development progresses.

## Learning Objectives

KubeGuardian is also a hands-on project for exploring Go application design, Kubernetes API integration, error handling, testing, concurrency, and production-oriented software practices.

## License

No license has been selected yet.
