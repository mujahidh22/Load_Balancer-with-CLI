# Load Balancer

A simple load balancer with cli implemented in Node.js and Express.


## Description

This project is a basic implementation of a load balancer using NodeJS and ExpressJS. The load balancer distributes incoming requests across multiple servers to ensure efficient utilization of resources and improved system reliability.


## Features

- Distributes incoming requests across multiple servers.
- Health checks to monitor server status.
- Simple CLI configuration for setting up server details.
- Logging of requests and errors for monitoring.

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/Load_balancer-with-CLI.git

   
2. **Install dependencies:**

   ```bash
   cd load-balancer
   npm install

2. **Run npm link to install the bin command globally:**

   ```bash
  npm link
   
## Usage

1. **Configure the load balancer using the CLI:**

   ```bash
   start-lb

 The CLI tool prompts the user for essential details, including:

- Number of servers
- Server URLs
- Health check endpoint
- Health check period
- This configuration ensures the load balancer has accurate information about available servers and their health.

   
2. **Send requests to the load balancer and observe the distributed load among servers.**

## Technical Details

### Round-Robin Load Balancing
The load balancer utilizes a round-robin algorithm to evenly distribute incoming requests among the available servers. This ensures each server gets an equal share of the load, preventing any single server from becoming a bottleneck.

### Health Checks
Periodic health checks are performed on each server to verify its availability. If a server fails a health check, it is temporarily removed from the rotation, preventing the load balancer from directing requests to an unhealthy server.

### Logging
The load balancer logs every incoming request and any encountered errors. This logging mechanism aids in monitoring and troubleshooting the system.

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.

## License
This project is licensed under the MIT. License.
Feel free to customize this further based on your specific implementation details and preferences.

