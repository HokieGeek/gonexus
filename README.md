# gonexus

Provides a go library for connecting to, and interacting with, Sonatype Nexus application such as Nexus Repository Manager and Nexus IQ Server.

## Organization
The library is broken into two packages. One for each application

### nexusrm [![GoDoc](http://godoc.org/github.com/hokiegeek/gonexus/rm?status.png)](http://godoc.org/github.com/hokiegeek/gonexus/rm)

Create a connection to an instance of Nexus Repository Manager
```go
import "github.com/hokiegeek/gonexus/rm"

rm, err := nexusrm.New("http://localhost:8081", "user", "password")
if err != nil {
    panic(err)
}
```

### nexusiq [![GoDoc](http://godoc.org/github.com/hokiegeek/gonexus/iq?status.png)](http://godoc.org/github.com/hokiegeek/gonexus/iq)

Create a connection to an instance of Nexus IQ Server
```go
import "github.com/hokiegeek/gonexus/iq"

iq, err := nexusiq.New("http://localhost:8070", "user", "password")
if err != nil {
    panic(err)
}
```

## The Fine Print
It is worth noting that this is **NOT SUPPORTED** by Sonatype, and is a contribution of HokieGeek
plus us to the open source community (read: you!)

Remember:

* Use this contribution at the risk tolerance that you have
* Do **NOT** file Sonatype support tickets related to this
* **DO** file issues here on GitHub, so that the community can pitch in
