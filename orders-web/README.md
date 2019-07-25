# Order Service

This is the Order service

Generated with

```
micro new github.com/songxuexian/gogomicro/orders-web --namespace=sxx.micro.book --alias=order --type=web
```

## Getting Started

- [Configuration](#configuration)
- [Dependencies](#dependencies)
- [Usage](#usage)

## Configuration

- FQDN: sxx.micro.book.web.order
- Type: web
- Alias: order

## Dependencies

Micro services depend on service discovery. The default is multicast DNS, a zeroconf system.

In the event you need a resilient multi-host setup we recommend consul.

```
# install consul
brew install consul

# run consul
consul agent -dev
```

## Usage

A Makefile is included for convenience

Build the binary

```
make build
```

Run the service
```
./order-web
```

Build a docker image
```
make docker
```