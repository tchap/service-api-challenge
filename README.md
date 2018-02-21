# Service API Challenge

I spend quite some time implementing internal services (APIs) in Go.
So I am asking myself a question - What is the most suitable technology for the job?

Here is what I need/want, basically:

1. Request/response communication pattern. I send a request, receive a response.
2. Code generation is really handy. I don't want to spend my life writing
   boilerplate code for unmarshalling HTTP response bodies in JSON.

## Challenge Specification

Let's imagine we are manufacturing simple IoT devices that have some state to be read/written.

Every device is assigned a globally unique identifier when it is manufactured.

Now we need some APIs to be able to:

1. Get device details by ID (e.g. device type, state schema perhaps?).
2. Read/write device state by ID, synchronously.

## Approaches Evaluated

I have decided to evaluate:

* [Swagger](https://goswagger.io/)
* [gRPC](https://grpc.io)

Please check the relevant subdirectories.