# free5gc-pcf-operator

[free5GC](https://www.free5gc.org/) is an open source 5G Core network implementation. This charmed
operator allows for automated deployment and lifecycle operations.

## Usage

```bash
juju deploy free5gc-pcf-operator --trust --channel=edge
```

## Relations

### Mongo DB

```bash
juju deploy mongodb-k8s
juju relate free5gc-pcf mongodb-k8s
```

## Image

- **[free5gc-pcf](https://github.com/gruyaume/free5gc-pcf-rock)**: ghcr.io/gruyaume/free5gc-pcf:1.1.1
