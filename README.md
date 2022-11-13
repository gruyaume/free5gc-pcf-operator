# free5gc-pcf-operator

[Free5gc](https://www.free5gc.org/) is an open source 5G Core network implementation. This charmed
operator allows for automated deployment and lifecycle operations.

## Usage

```bash
juju deploy free5gc-pcf --trust
```

## Relations

### Mongo DB

```bash
juju deploy mongodb-k8s
juju relate free5gc-pcf mongodb-k8s
```

## Image

- **free5gc-pcf**: towards5gs/free5gc-pcf:v3.2.0
