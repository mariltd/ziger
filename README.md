# Ziger

**Ziger** is a blazing-fast, minimal HTTP/1.1 web server written in Zig. Designed as a high-performance alternative to nginx for specific use cases, it leverages Zig's zero-overhead abstractions for raw speed—aiming for 100k+ req/s on commodity hardware.

![Ziger Banner](https://via.placeholder.com/1200x400/000000/ffffff?text=Ziger+-+Blazing+Fast+Zig+HTTP+Server)

## Why We Better Than Nginx
- Cool name
- Pure Zig standard library—no external deps for core server.
- Async connection handling with threading.
- Basic routing (`/`, `/metrics` JSON endpoint).
- Static file serving from `./public/`.
- Zero-allocation hot path where possible.
- Cross-platform (Linux/macOS/Windows).

## Quick Go-To

1. **Install Zig** (0.15+): https://ziglang.org/download/
2. **Clone & Build**:
   ```bash
   git clone <your-repo> ziger
   cd ziger
   zig build run
3. **Enjoy**:
   ```bash
   curl http://localhost:8080        # Hello, Ziger!
   curl http://localhost:8080/metrics # {"reqs":1,"uptime":123}
Ziger is still UNDER CONSTRUCTION!
