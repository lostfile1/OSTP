# The Open Spacial Traversal Protocol (OSTP)
Open Spatial Traversal Protocol is an open protocol for a metaverse that respects consumer and corporate interests. The OSTP prevents users of a metaverse/metaverses from being locked into a specific hardware path. The Metaverse was iOS, Holodeck is Android.

# The Point of this project

Create a protocol that cannot be locked down while still drawing in corporate interests, otherwise it will die like other projects like opensim and janusweb 

# Architecture Overview
```
+-------------------+         1. Portal Handshake (HTTPS)        +-------------------+
|   Home Node /     | -----------------------------------------> |   Target Host     |
|   Current Node    | <----------------------------------------- |   Node (World B)  |
+-------------------+      2. Policy & Capability Offer          +-------------------+
         |                                                                 ^
         | 3. Client Redirect + Signed Session Ticket                      |
         v                                                                 |
+-------------------+         4. Real-Time Spatial Sync            +-------------------+
|   User Client     | =========================================>   |   Target Host     |
| (Browser/Native)  |     (WebSocket / WebRTC / QUIC Stream)       |   Simulation      |
+-------------------+                                              +-------------------+

```

# Some Examples of Universal Routing Interface (URI) Addresses

### Example of a User Or AI agent
```
ostp://alice@home-node.example
```

### Example of a Portal
```
ostp://world-b.example/plaza?spawn=north
```

We are currently looking for collaborators for this project 