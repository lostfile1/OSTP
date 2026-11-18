# The OSTP protocol
Open Spatial Traversal Protocol A Protocol for a metaverse that prevents a walled garden situation, but still respects consumer and corporate interests 

# The Point of this project

To create a protocol that cant be garden walled but still draw in corporate interests either wise it will die like other projects like opensim and janusweb 

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

# Some Examples of URI addresses

### Example of a User Or AI agent
```
ostp://alice@home-node.example
```

### Example of a Portal
```
ostp://world-b.example/plaza?spawn=north

```
