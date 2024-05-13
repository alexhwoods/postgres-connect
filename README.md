This application is for testing connection to a Redis instance.

It's common for Redis instances to be deployed inside a VPC with authentication off. If you run this container on a network that can access the IP address of the Redis instance, it should work.

Otherwise, it should panic.

```go
REDIS_ADDR=127.0.0.1:6379 go run main.go
```