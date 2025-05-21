## DEPRECATION ANNOUNCEMENT

This repository now no longer houses the latest RHDH helm charts.
Our new CI Helm charts can be accessed at quay.io/rhdh/chart. The scripted installation has been updated to reflect this change.

Soon the installation instructions and script will also no longer be accessible in this repository. More information will be shared at a later date.

## Scripted installation

To [install](./install.sh) from a Helm Chart Repository, run the following commands:

```
cd /tmp
# Create or select a namespace
# Install the chart repo
# Install the chart, then update the clusterRouterBase
curl -sSLO https://raw.githubusercontent.com/rhdh-bot/openshift-helm-charts/rhdh-1-rhel-9/installation/install.sh && chmod +x install.sh
./install.sh 1.7-61-CI --namespace rhdh-1-7-61-ci
```

That's it! 