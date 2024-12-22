# Custom Redis Server

A custom implementation of a Redis server built from the ground up. This project is a TCP server that handles core Redis functionalities such as basic command handling, RDB file persistence, replication, transactions, and streams. It's designed to be a minimal yet scalable solution for handling Redis-like operations.

## 🚀 Features

- **Basic Commands**: Supports PING, ECHO, SET & GET operations.
- **Client Concurrency**: Handles multiple clients simultaneously with efficient concurrency management.
- **Key Expiry**: Implements key expiry mechanism for automatic data expiration.
- **RDB Persistence**: Reads and writes RDB files to persist data efficiently.
- **Replication (In Progress)**: Adding support for replication across multiple Redis instances.
- **Transactions (In Progress)**: Implementing transaction support for atomic command execution.
- **Streams (In Progress)**: Building stream features for continuous data handling.

## 📂 Project Structure
```bash
.
├── app
│   ├── consts.js          # Constant values used across the app
│   ├── main.js            # Main server logic
│   ├── parseRDB.js        # RDB persistence handling
├── .gitattributes         # Git configuration for attributes
├── .gitignore             # Git configuration to ignore specific files
├── codecrafters.yml       # Codecrafters challenge configuration
├── package-lock.json      # Auto-generated lock file for dependencies
├── package.json           # Project dependencies and scripts
├── README.md              # Project documentation
└── your_program.sh        # Shell script to run the program


```
## 🛠️ Getting Started

### Prerequisites

- **Node.js**: Ensure you have [Node.js](https://nodejs.org/) installed on your machine.
- **Git**: Version control system to clone this repository.

### Installation & Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/redis-server.git
   ```
2. Navigate to the project directory:

   ```bash
   cd redis-server
   ```
3. Install dependencies:

   ```bash
   npm install
   ```
4. Run the Redis server:

   ```bash
   node app/main.js
   ```
## 🚦 Usage

**PING:**

```bash
redis-cli PING
```
Output: `PONG`

**SET & GET:**

```bash
redis-cli SET key "value"
redis-cli GET key
```
Output: `"value"`

**ECHO:**
```bash
redis-cli ECHO "Hello, Redis!"
```
Output: `"Hello, Redis"!`

## 🗂️ RDB Persistence
The Redis server supports RDB persistence for saving data to disk. It reads keys, string values, and handles key expiry from an RDB file, ensuring data recovery after a restart.

## 🌟 Completed Stages

- Bound to port for client connections
- Responded to PING and multiple PINGs
- Implemented ECHO, SET, and GET commands
- Handled concurrent clients
- Added expiry functionality for keys
- RDB persistence: Configured RDB, read keys/values, and handled key expiry

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## 👤 Author

   **Divyanshu** - [Your GitHub Profile](https://github.com/dsthakur402)

