# WobotRelay-App

**Note: This is a private repository. Please contact Shivang @shivang0070 for access.**

**WobotRelay-App** is a robust and efficient application designed to facilitate WebSocket communication between clients and a server. It provides a seamless way to manage client-server interactions, configuration management, and real-time data exchange.

## Features

- WebSocket communication
- Client-server interaction
- Configuration management
- Real-time data exchange
- API endpoints for client management
- Persistent client state using BoltDB

## Installation Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/shivang0070/WebSocket-App.git
   cd WebSocket-App
   ```

2. Install dependencies:
   ```bash
   go mod tidy
   ```

3. Build the project:
   ```bash
   go build -o websocket-app
   ```

## Usage

1. Start the server:
   ```bash
   ./websocket-app
   ```

2. Connect a client to the server using a WebSocket client (e.g., a web browser or a custom client application).

3. Interact with the server using the available API endpoints.

## API Documentation

### GET /clients

Retrieve a list of all connected clients.

### GET /clients/:clientID

Retrieve detailed information about a specific client.

### GET /clients/:clientID/paths

Retrieve the paths configuration for a specific client.

### POST /clients/:clientID/name

Set the name of a specific client.

### POST /clients/:clientID/paths

Add or update a path configuration for a specific client.

### DELETE /clients/:clientID/paths/:pathName

Delete a path configuration for a specific client.

### POST /clients/:clientID/reload

Trigger a reload of the configuration for a specific client.

## Configuration

The project uses a `config.yaml` file for configuration management. The structure of the file is as follows:

```yaml
server:
  port: 8787
  api_key: your-super-secret-key

database:
  file: server_clients.db
  bucket: Clients
```

## Running the Project

1. Ensure that the `config.yaml` file is properly configured.

2. Start the server:
   ```bash
   ./websocket-app
   ```

3. Connect clients and interact with the server using the available API endpoints.

## Development Setup

1. Install Go (version 1.16 or higher) from the official website: https://golang.org/dl/

2. Clone the repository and navigate to the project directory:
   ```bash
   git clone https://github.com/shivang0070/WebSocket-App.git
   cd WebSocket-App
   ```

3. Install dependencies:
   ```bash
   go mod tidy
   ```

4. Build the project:
   ```bash
   go build -o websocket-app
   ```

5. Start the server:
   ```bash
   ./websocket-app
   ```

## Contributing

We welcome contributions to the project! Please follow these guidelines when contributing:

1. Fork the repository and create a new branch for your feature or bugfix.
2. Write clear and concise commit messages.
3. Ensure that your code follows the project's coding standards.
4. Submit a pull request with a detailed description of your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Contact Information

For any questions or inquiries, please contact Shivang at @shivang0070.
