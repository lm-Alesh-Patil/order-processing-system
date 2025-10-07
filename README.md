# order-processing-system
Order Processing System (with RabbitMQ)

# Project Structure
go-rabbitmq-orders/
├── cmd/
│   ├── api/
│   │   └── main.go          # Starts REST API (producer)
│   └── worker/
│       └── main.go          # Starts background worker (consumer)
├── internal/
│   ├── rabbitmq/
│   │   └── connection.go    # Common RabbitMQ connection
│   ├── handler/
│   │   └── order_handler.go # HTTP handler
│   ├── service/
│   │   └── order_service.go # Business logic
│   ├── repository/
│   │   └── order_repo.go    # DB simulation / store
│   └── model/
│       └── order.go         # Order model struct
├── go.mod
└── go.sum
