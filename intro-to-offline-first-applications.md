Offline first application
—
Max Gfeller

What is it ?
Why we should do it ?
How to ?

Intro
Web technologie
Tooling
Our approach

PWA (progressive web application)
fast (should load instantly)
integrated
reliable
engaging

Opinion: Actually most of app who claims are pwa, are mostly pw.

PWA for people far in a cave ?
Have you already tryied working on a train ?

Why are native application better ?

Webapp <-> Service Worker <-> Server

How to respond to request ? Cache api

Background …
allow to delay send of the request
have cons : introduce complexity, business logic is leaked into the cache mechanism

Cookie : 4096 bytes
WebStorage : 10mb
Indexed DB : no limit

LRU policy !
Use Persistent storage.

How is persistent storage granted ?
safari : not supported
firefox : ask the user
chrome : look at several metrics


Tooling

Workbox by google (lot of caching strategy implemented)

Replicating Database : PouchDB , Replicache

Firebase
Realm
AWS Amplify

Eremite.js
backend agnostic (rest api, graphql api, …)