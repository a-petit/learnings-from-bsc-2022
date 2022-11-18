# Appetizer


## Ted Neward - Orleans

Orleans is a cross-platform framework for building distributed applications based on the "actor model".

Each actor has its own state
Only an actor can modify its own state
Benefits of such models is that you avoid problems with taking lock, ...

An alternative to Orleans is Akka.net

An actor as an id, logic, state
An object as an implicit id, logic, state

Resources:
- https://github.com/tedneward/Demo-Orleans
- https://learn.microsoft.com/en-us/dotnet/orleans/

## Ian Cooper - Outbox

Brighter, open source project
Outbox / inbox pattern
Achieve "At least once"

He use a nice tests.http to run some http requests.

> appLaunchSettings.json can expose several profiles.
>
> This can be great to have a local fast mode?

Resources:
- Dapper: https://github.com/DapperLib/Dapper
- Polly (retry framework in dotnet)