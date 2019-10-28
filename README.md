# DL_HW3

```mermaid
graph LR
A[Video Stream] -->B(dBODet)
subgraph Detection App
B --> C(Detect)
C -->|Writes to DB| D(Detection metadata)
C -->|Writes to DB| E(User logs)
end
D-->|Reads Metadata| F(User)
A-->|Reads Stream| F
```
