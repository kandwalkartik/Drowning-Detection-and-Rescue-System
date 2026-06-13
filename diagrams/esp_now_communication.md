# Current ESP-NOW Communication Architecture

Status: Implemented diagram.

This diagram shows the current ESP32 and ESP-NOW based rescue communication concept, including communication toward a control station.

```mermaid
flowchart LR
    A["Wearable Node A<br/>ESP32"] <-->|"ESP-NOW Peer-to-Peer Rescue Message"| B["Wearable Node B<br/>ESP32"]
    A --> C["Control Station / Monitoring Unit"]
    B --> C
    C --> D["Event Alert Display"]
    D --> E["Rescue / Monitoring Team"]
```

Note: This diagram does not claim implemented infrastructure nodes, dynamic relay selection, distributed storage, or shoreline-scale routing.
