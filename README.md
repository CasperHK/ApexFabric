# ApexFabric
ApexFabric is a production-hardened meta-framework designed for the 2026 enterprise landscape. By unifying the extreme request throughput of Go Fiber with the type-safe, SQL-first efficiency of Go Bun, ApexFabric provides a standardized foundation for large-scale distributed systems.
🛡️ Why ApexFabric?
In an enterprise environment, raw speed isn't enough—you need structure, observability, and safety. ApexFabric enforces architectural discipline while maintaining the "low-boilerplate" philosophy of Go.
⚡ Velocity at Scale: Leverages Fiber's fasthttp core to handle millions of concurrent connections with zero allocation overhead.
💎 Type-Safe Persistence: Uses Bun to eliminate the "black box" of heavy ORMs, providing clear, high-performance SQL generation that your DBAs will love.
🏗️ Layered Architecture: Out-of-the-box support for Clean Architecture and Domain-Driven Design (DDD). Business logic stays pure, isolated from the transport and data layers.
📊 Observability First: Native integration with OpenTelemetry, structured logging via slog, and real-time health metrics.
🚀 Quick Start (2026 Standard)
Initialize your first enterprise service in seconds:
bash
# Install the Apex CLI
go install github.com

# Create a new service with Clean Architecture scaffold
apex new my-service --db postgres --auth oidc
請謹慎使用程式碼。

🧱 Core Architecture
ApexFabric organizes your enterprise app into three immutable layers:
Transport Layer (Fiber): High-speed entry points, automated OpenAPI/Swagger generation, and standardized error handling.
Domain Layer (Pure Go): Where your business logic lives. Zero dependencies on Fiber or Bun.
Data Layer (Bun): Type-safe repositories, automated migrations, and connection pooling optimized for high-traffic RDS/PostgreSQL clusters.
🌐 Enterprise Ecosystem
ApexFabric is more than a library; it’s a standard. It includes built-in modules for:
Identity: Pre-configured OIDC and JWT middleware.
Resilience: Native Circuit Breakers and Retries via Go-Resilience.
Messaging: First-class support for Kafka and RabbitMQ events.
Read the Docs | Explore the Recipe | View on GitHub
