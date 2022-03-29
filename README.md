# FauxpenShift

This cli utility creates a Kubernetes cluster using [µShift](https://microshift.io/docs/home/) (Known as "Microshift". A version of OpenShift that runs in a container) and a custom version of the [OpenShift Router](https://github.com/openshift/router) on top of it. This is useful for when you want to test your applications using OpenShift, but [CRC](https://developers.redhat.com/products/codeready-containers/overview) is too heavy.

Check out the usage guide for your platfrom/runtime for specifics:

* [Linux and Podman](docs/podmanLinux.md)
* [Linux and Docker](docs/dockerLinux.md)
* [Mac and Podman](docs/podmanMac.md)
* [Mac and Docker](docs/dockerMac.md)

# Prerequisites

At a minimum

* Docker or Podman (Docker is experimental, but should work)
* Access to Nip.io

You will also have to satisfy all the prerequisites of µShift. You will need to pay attention to the [Appliation Development](https://microshift.io/docs/getting-started/#using-microshift-for-application-development) SELinux setup and the [Firewall Rules](https://microshift.io/docs/getting-started/#deploying-microshift) setup as well.

> **NOTE** Don't actually run Microshift, just do the prereqs

If you are using Docker Desktop, please use the [same guidance as KIND](https://kind.sigs.k8s.io/docs/user/quick-start/#settings-for-docker-desktop) with respect to resources (you gotta bump them up)

