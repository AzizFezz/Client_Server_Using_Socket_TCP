# Distributed Application with TCP Communication

This project involves the creation of a connected (TCP) distributed application, allowing clients to request the execution of specific services from a server.

## Client Process

The client process must provide a Text-based User Interface (TUI) allowing:

- Authentication (username + password) with the server.
- Repeatedly:
  - Viewing the list of services offered by the server.
  - Choosing a service and sending the service request.
  - Viewing the results returned by the server.

Repeat until the choice is 'exit'.

## Server Process

The server process (parallel server) provides at least the following services:

1. Displays the current date (day/month/year) and time (hour : minutes : seconds) from the server's system clock.
2. Displays the list of files in the current directory.
3. Displays the content of a file in the current directory.
4. Displays the elapsed time since the current client connection began.

## Implementation

1. **Client Program (`Cl.c`)**: Implement the client program with the specified functionalities.

2. **Server Program (`Ser.c`)**: Implement the server program with multi-threading to handle multiple clients simultaneously.

3. **Automation Script (`script.sh`)**: Provide a shell script configured with the names of the source codes to automate the compilation and linking steps.

## Usage

To compile the project, use the following command:

```bash
user@linux:~/Project$ ./script.sh
```

To launch the server, use the following command:

```bash
user@linux:~/Project$ ./serveurTCP <port>
```

To launch the client, use the following command:

```bash
user@linux:~/Project$ ./clienTCP <server_address> <port>
```

Make sure to replace <port> and <server_address> with the appropriate values.
