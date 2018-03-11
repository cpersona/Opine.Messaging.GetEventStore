# Opine.Messaging.GetEventStore
EventStore adapter for the Opine framework. 

## Getting started

### Cloning and building

Clone the repository and Opine. Use the `dotnet build` command to build the projects.

```
git clone https://github.com/cpersona/Opine
git clone https://github.com/cpersona/Opine.Messaging.GetEventStore
cd Opine.Messaging.GetEventStore
dotnet build
```

## Motivation

Opine (https://github.com/cpersona/Opine) is a CQRS and Event Sourcing framework. One of the core concepts of Opine is the _IMessageStore_ interface which provides abstracted methods of reading and writing messages (events and commands). Opine also provides the _ISnapshotStore_ interface for reading and writing snapshots of aggregate roots. 

EventStore (https://eventstore.org/) is an open source implementation of an event store created by Greg Young. It provides the ability to read and write streams of events in a transactional manner and is a strong foundation for a CQRS and Event Sourcing based system. 

**Opine.Messaging.GetEventStore** provides implementations of Opine Framework's _IMessageStore_ and _ISnapshotStore_ using EventStore's .NET Core API to provide an easy drop-in implementation.

## Technologies
* .NET Core 2.0
* C# 7
* Event Store (https://geteventstore.com)

## Optional Technologies
* N/A

## Third-party Libraries
* Opine (https://github.com/cpersona/Opine)
* EventStore.ClientAPI.NetCore (https://github.com/EventStore/ClientAPI.NetCore)

## References
* EventStore Documentation (https://eventstore.org/docs/)
