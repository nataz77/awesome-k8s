# Awesome Microservices on K8S components

Here's a list of various [CNCF](https://www.cncf.io/projects/) and non-CNCF projects and components we use to build cloud-native microservices architectures.

## Kubernetes distributions
- [RKE](https://rancher.com/products/rke/) is a CNCF-certified Kubernetes distribution that runs entirely within Docker containers. It works on bare-metal and virtualized servers. RKE solves the problem of installation complexity, a common issue in the Kubernetes community.
- [K3s](https://k3s.io/) is a highly available, certified Kubernetes distribution designed for production workloads in unattended, resource-constrained, remote locations or inside IoT appliances.
- [Metal³](https://metal3.io/) exists to provide components that allow you to do bare metal host management for Kubernetes.  works as a Kubernetes application, meaning it runs on Kubernetes and is managed through Kubernetes interfaces.

## Kubernetes orchestration management
- [Rancher](https://rancher.com/) is multi-cluster container management system, built to give team members a 360&deg; view on the cluster.
- [Kubernetes dashboard](https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/) is a web-based Kubernetes user interface. You can use Dashboard to deploy containerized applications to a Kubernetes cluster, troubleshoot your containerized application, and manage the cluster resources.

## Kubernetes infrastructure management
- [Crossplane](https://crossplane.io/) is an open source Kubernetes add-on that supercharges your Kubernetes clusters enabling you to provision and manage infrastructure, services, and applications from kubectl.

## Other Kubernetes platforms
- [KubeEdge](https://kubeedge.io/en/) is a fully open, scalable & portable Kubernetes based Edge Computing platform.

## Kubernetes tooling
- [Kured](https://github.com/weaveworks/kured) is a Kubernetes daemonset that performs safe automatic node reboots when the need to do so is indicated by the package management system of the underlying OS.
- [kubectl-who-can](https://github.com/aquasecurity/kubectl-who-can) is a tool that shows which subjects have RBAC permissions to VERB [TYPE | TYPE/NAME | NONRESOURCEURL] in Kubernetes.

## Container registry 

- [Harbor](https://goharbor.io/) is an open source registry that secures artifacts with policies and role-based access control, ensures images are scanned and free from vulnerabilities, and signs images as trusted.

## Container registry tooling
- [Sinker](https://github.com/plexsystems/sinker) is an open source tool that syncs container images from one registry to another. This is useful in cases when you rely on images that exist in a public container registry, but need to pull from a private registry.

## Storage management and orchestration
- [Rook](https://rook.io/) is a cloud-native storage orchestrator platform to enable highly available, durable storage in your Kubernetes cluster.
- [Ceph CSI](https://github.com/ceph/ceph-csi) is an interface between CSI enabled Container Orchestrator (CO) and Ceph cluster. It allows dynamically provisioning Ceph volumes and attaching them to workloads.
- [Longhorn](https://rancher.com/products/longhorn/) is an official CNCF project that delivers a powerful cloud-native distributed storage platform for Kubernetes that can run anywhere.
- [OpenEBS](https://openebs.io/) builds on Kubernetes to enable Stateful applications to easily access Dynamic Local PVs or Replicated PVs. By using the Container Attached Storage pattern users report lower costs, easier management, and more control for their teams.

## GitOps
- [Flux](https://fluxcd.io/) is a tool that automates the deployment of containers to Kubernetes. It fills the automation void that exists between building and monitoring.
- [Helm Operator](https://docs.fluxcd.io/projects/helm-operator/en/stable/) is a Kubernetes operator, allowing one to declaratively manage Helm chart releases. Combined with Flux this can be utilized to automate releases in a GitOps manner, but the use of Flux is not strictly necessary

## [Service Mesh](https://servicemesh.io/) 
- [Istio](https://istio.io/) is an open platform for providing a uniform way to integrate microservices, manage traffic flow across microservices, enforce policies and aggregate telemetry data.
- [Linkerd](https://linkerd.io/) is a service mesh for Kubernetes. It makes running services easier and safer by giving you runtime debugging, observability, reliability, and security—all without requiring any changes to your code.
- [Kuma](https://kuma.io/) is a modern control plane for Microservices & Service Mesh for both K8s and VMs, with support for multiple meshes in one cluster. It provides out-of-the-box L4 + L7 policy architecture to enable zero trust security, observabilty, discovery, routing and traffic reliability in one click.
- [Open Service Mesh (OSM)](https://openservicemesh.io/) is a lightweight, extensible, cloud native service mesh that allows users to uniformly manage, secure, and get out-of-the-box observability features for highly dynamic microservice environments. 

## Pub-sub
- [Nats](https://nats.io/) is a simple, secure and high performance open source messaging system for cloud native applications, IoT messaging, and microservices architectures.

## Ingress controllers
- [NGINX Ingress Controller](https://kubernetes.github.io/ingress-nginx) provides enterprise‑grade delivery services for Kubernetes applications
- [Kong Ingress Controller](https://github.com/Kong/kubernetes-ingress-controller) offers all the common Kong feature such as plugins, health checking, load balancing and more in Kong for Kubernetes Services, all using Custom Resource Definitions(CRDs) and Kubernetes-native tooling.
- [Traefik](https://traefik.io) is a modern HTTP reverse proxy and load balancer that makes deploying microservices easy
- [HAProxy Ingress controller](https://haproxy-ingress.github.io/) is a fast and reliable TCP and HTTP reverse proxy and load balancer. HAProxy Ingress carefully builds an optimized HAProxy configuration, which allows thousands of requests per second per proxy, despite the size of your cluster, with a very low latency.
- [Istio](https://istio.io/) is an open platform for providing a uniform way to integrate microservices, manage traffic flow across microservices, enforce policies and aggregate telemetry data.
- [Skipper](https://opensource.zalando.com/skipper/kubernetes/ingress-controller/) is the open-source ingress controller that powers 112 Kubernetes clusters at Zalando, which offers HTTP router and reverse proxy for service composition, designed as a library to build your custom proxy.

## Monitoring, logging, observability and tracing
- [Prometheus](https://prometheus.io/) is an open-source systems monitoring and alerting toolkit originally built at SoundCloud.
- [Jaeger](https://www.jaegertracing.io/) is a distributed tracing system released as open source by Uber Technologies. It is used for monitoring and troubleshooting microservices-based distributed systems, including distributed context propagation, distributed transaction monitoring, root cause analysis, service dependency analysis, performance/latency optimization
- [Grafana](https://grafana.com/) has become the world’s most popular technology used to compose observability dashboards with everything from Prometheus & Graphite metrics, to logs and application data to power plants and beehives.
- [Fluentd](https://www.fluentd.org/) is an open source data collector for unified logging layer.
- [OpenTracing](https://opentracing.io) is comprised of an API specification, frameworks and libraries that have implemented the specification, and documentation for the project. OpenTracing allows developers to add instrumentation to their application code using APIs that do not lock them into any one particular product or vendor.

## Security
- [Falco](https://falco.org/) is an open source runtime security tool that parses Linux system calls from the kernel at runtime, and asserts the stream against a powerful rules engine. It can be used for Kubernetes runtime security.
- [CloudSploit](https://github.com/aquasecurity/cloudsploit) by Aqua is an open-source project designed to allow detection of security risks in cloud infrastructure accounts, including: Amazon Web Services (AWS), Microsoft Azure, Google Cloud Platform (GCP), Oracle Cloud Infrastructure (OCI), and GitHub. These scripts are designed to return a series of potential misconfigurations and security risks.
- [kube-hunter](https://github.com/aquasecurity/kube-hunter) is a tool that hunts for security weaknesses in Kubernetes clusters. The tool was developed to increase awareness and visibility for security issues in Kubernetes environments.
- [kube-bench](https://github.com/aquasecurity/kube-bench) is an application that checks whether Kubernetes is deployed securely by running the checks documented in the CIS Kubernetes Benchmark.

## CI/CD
- [Tekton](https://tekton.dev/) is a powerful and flexible open-source framework for creating CI/CD systems, allowing developers to build, test, and deploy across cloud providers and on-premise systems.
- [Keptn](https://keptn.sh/) is an event-based control plane for continuous delivery and automated operations for cloud-native applications.
- [Buildpacks](https://buildpacks.io/) transforms your application source code into images that can run on any cloud. 
- [Argo](https://argoproj.github.io/) provides open source Kubernetes native workflows, events, CI and CD
- [Trivy](https://github.com/aquasecurity/trivy) is a simple and comprehensive vulnerability scanner for containers and other artifacts, suitable for CI.

## Events
- [KEDA](https://keda.sh/) is a single-purpose and lightweight component that can be added into any Kubernetes cluster. KEDA works alongside standard Kubernetes components like the Horizontal Pod Autoscaler and can extend functionality without overwriting or duplication to provide event driven autoscaling
- [CloudEvents](https://cloudevents.io/) is a specification for describing event data in common formats to provide interoperability across services, platforms and systems.

## Function as a service
- [OpenFaaS](https://www.openfaas.com/) makes it easy for developers to deploy event-driven functions and microservices to Kubernetes without repetitive, boiler-plate coding. Package your code or an existing binary in a Docker image to get a highly scalable endpoint with auto-scaling and metrics.

## Testing
- [ChaosKube](https://github.com/linki/chaoskube) is a tool that periodically kills random pods in your Kubernetes cluster to test resiliency.
- [Kboom (WIP)](https://github.com/mhausenblas/kboom) is a tool that allows you to create short-term load for scale testing and long-term load for soak testing. Supported load out of the box for scale testing are pods and custom resources via CRDs for soak testing is planned. (this is WIP)
- [kube-advisor](https://github.com/Azure/kube-advisor) is a diagnostic tool for Kubernetes clusters. At the moment, it returns pods that are missing resource and request limits.

