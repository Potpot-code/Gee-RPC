# Gee-RPC

Gee-RPC is a lightweight and high-performance RPC (Remote Procedure Call) framework implemented from scratch in Go. Designed with simplicity and efficiency in mind, Gee-RPC provides essential features for building distributed systems, including service registration, message encoding, high-performance clients, timeout handling, HTTP protocol support, load balancing, and service discovery with a registry center.

## Features

- **Service Registration**: Easily register services and methods for remote invocation.
- **Message Encoding**: Efficient encoding and decoding of messages for communication between client and server.
- **High-Performance Client**: A lightweight and fast client for making RPC calls.
- **Timeout Handling**: Built-in timeout mechanisms to prevent hanging requests.
- **HTTP Protocol Support**: Seamlessly supports HTTP as a transport protocol for RPC communication.
- **Load Balancing**: Distributes requests across multiple service instances for better performance and reliability.
- **Service Discovery & Registry Center**: Automatically discover and register services in a distributed environment.

## Getting Started

### Prerequisites

- Go 1.20 or higher.

### Installation

Clone the repository:

```bash
git clone https://github.com/Potpot-code/Gee-RPC.git
cd Gee-RPC
```

### Usage

#### 1. Start the Registry Center

The registry center is responsible for service discovery and registration. Start it to enable service registration and discovery.

#### 2. Register a Service

Define and register a service on the server. The server will listen for incoming RPC requests and handle them accordingly.

#### 3. Create a Client

Create a client to call the remote service. The client supports both direct connections and load-balanced requests.

#### 4. Run with Load Balancing

Use the `XClient` for load balancing across multiple servers. Choose between round-robin or random selection strategies.

#### 5. HTTP Protocol Support

Start an HTTP server to handle RPC requests over HTTP. Clients can send requests using HTTP POST methods.

### Configuration

- **Timeout**: Set timeout for client calls to prevent hanging requests.
- **Load Balancing Strategy**: Choose between round-robin or random selection for distributing requests.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## Acknowledgments

- Inspired by Go's standard library and other open-source RPC frameworks.
- Special thanks to the Go community for their invaluable resources and support.

---

Happy coding with Gee-RPC! 🚀
