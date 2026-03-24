# GO-RAT
    GO-RAT is a simple cross platform remote access tool (RAT) framework with a command-and-control server and client agent,
    designed for learning/testing in controlled environments.

<img width="1136" height="353" alt="image" src="https://github.com/user-attachments/assets/ca6768ee-d8fe-4315-81ef-b4518249ca2b" />

## Build
    - change ip and port in client.go and server.go
    - go build mod init gorat
    - go get github.com/kbinani/screenshot
    - go build client.go
    - go build server.go

## Server commands
    - `targets` - show active session list
    - `sessionN` - connect to session N (example `session0`)
    - `exit` - stop server
    
    Inside/Shell session:
    
    - `q` - quit session / return to server menu
    - `info` - gather client info (username/hostname/MAC)
    - `download <file>` - download remote file from client
    - `upload <file>` - upload server file to client
    - `screen` - capture screenshot

## Features
    - Multiple client session handling
    - Unique client dedup using hostname/MAC/username/IP key
    - Session command shell per client
    - File upload/download between server & client
    - Screenshot
    - Auto reconnect
    - More features will be added

## Important
    This code is for educational purposes only. Use only on systems you own or have explicit permission to test. Unauthorized use is illegal.
