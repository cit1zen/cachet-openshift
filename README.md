# Cachet templates for OpenShift 3

This is the unofficial repository containing templates and imagestreams that add [Cachet](https://github.com/cachethq/Cachet) to your OpenShift project.

[Cachet](https://github.com/cachethq/Cachet) is a beautiful and powerful open source status page system, a free replacement for services such as StatusPage.io, Status.io and others.

For full documentation, visit the [Installing Cachet with Docker](https://docs.cachethq.io/docs/get-started-with-docker) page.

## Quickstart

1. Clone this repository
```
git clone https://github.com/cit1zen/cachet-openshift.git
```

2. Move into repository
```
cd cachet-openshift
```

3. Add imagestream to your OpenShift project
```

oc create -f imagestreams/cachet-official.yaml
```

4. Add template to your OpenShift project
```
oc create -f templates/cachet.yaml
```

5. Deploy Cachet
* Deployment using WebUI
* Deployment using CLI