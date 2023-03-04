# Playing With Weaver

Weaver is Google Clouds framework for managing distributed systems locally and
in the cloud.

https://serviceweaver.dev/docs.html

## Prerequisites:

weaver:
```
go install github.com/ServiceWeaver/weaver/cmd/weaver@latest
```

## To Run

Generate weaver runtime code

```
weaver generate .
```

### Single process:

```
go run .
```

To view:
```
weaver single status
```
local dashboard
```
weaver single dashboard
```

### Multi process


```
go build . # Build binary
weaver multi deploy weaver.toml
```

To view:
```
weaver multi status
```
local dashboard
```
weaver multi dashboard
```

