# Architecture Context

```mermaid
flowchart LR
    Customer[Customer] --> Channels[Digital Channels]
    Merchant[Merchant] --> API[API Platform]
    Channels --> API
    API --> CIAM[CIAM]
    API --> Domain[Domain Services]
    Domain --> Core[Core / Processor]
    Domain --> Events[Event Platform]
    Events --> Data[Data Platform]
    Data --> Analytics[Analytics / AI]
```
