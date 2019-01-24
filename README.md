# JBOK #
Go to the [**microsite**](https://c-block.github.io/jbok/) for more information.
## TL;DR ##
```console
$ helm install chart
```
## Prerequisites ##

 - Kubernetes 1.8

## Install ##
You can specify each parameter using the `--set key=value[,key=value]` argument to helm install as follows:

```console
$ helm install chart --name my-release
    --set chain.node=1
```
or provide a YAML file that specifies the values you want:

```console
$ helm install chart --name my-release -f override-values.yaml 
```
## Upgrade ##
To upgrade the my-release deployment:

```console
$ helm upgrade my-release chart -f override-values.yaml
```
## Uninstall ##
To uninstall/delete the my-release deployment:

```console
$ helm delete my-release
```

The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration ##
To be continued.

| Parameter | Description | Default |
|-----------|-------------|---------|
|`chain.nodes`|number of nodes for the blockchain network|1|