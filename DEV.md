How to compile examples for windows
--------------------------

env GOOS=windows GOARCH=386 go build -o bin/opcua.exe examples/read/read.go
env GOOS=windows GOARCH=amd64 go build -o bin/opcua.exe examples/read/read.go

Usage
------

You can use flags from command line like:

write.exe -endpoint opc.tcp://127.0.0.10:5000 -node 'ns=0;i=2261' -value 'Active'

Available flags are in the code. Docuemntation about flags is here: https://golang.org/pkg/flag/

