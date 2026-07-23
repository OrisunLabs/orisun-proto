# Orisun Protocol Buffer Definitions

This repository contains the shared Protocol Buffer definitions for the Orisun Event Store.

## Contents

- `eventstore.proto` - Event Store service definitions
- `admin.proto` - Admin service definitions

## Usage

### Go

From the root of the main Orisun checkout, generate Go code with:

```bash
./scripts/generate_go_proto.sh
```

In the main Orisun repository this writes both messages and service stubs to
`orisun/grpcapi`. Other Go modules may override the Go package mapping when
generating their own client bindings.

### Java

The proto files are used by the Java client's Gradle build process. See [orisun-client-java](https://github.com/OrisunLabs/orisun-client-java) for usage.

### Node.js

The Node.js client has its own copy of the proto files. See [orisun-node-client](https://github.com/OrisunLabs/orisun-node-client).

## License

MIT License - see [LICENSE](LICENSE) for details.

## Repository

https://github.com/OrisunLabs/orisun-proto
