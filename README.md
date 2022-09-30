# kschain-resolver
<img src="https://user-images.githubusercontent.com/72974863/192973196-cb5b248b-d307-4fce-bae6-f3525681ea85.png" width=70% height=70%>


## 1. Specification
### 1.1 KSChain DID Method Specification
+ [KSChain DID Method Specification](https://tangy-gallium-b9b.notion.site/DID-Method-Specification-KSChain-7a77664f1eae47769692f4ff2d029fe0)
### 1.2 Reference
+ [W3C DID Specification Registries](https://www.w3.org/TR/did-spec-registries/)
+ [W3C Decentralized Identifier v1.0](https://w3c.github.io/did-core/)
+ [W3C Decentralized Identifier Resolution v0.2](https://w3c-ccg.github.io/did-resolution/)


## 2. Example DIDs
```did:kscirc:k12NqvVM9BX6AaMjPK1hUTUkKBWPBAUXAszTxdx7jDZPv4iqCZ1D```
```did:kscirc:k17qQYbApdfTdxsrS77k3sbFmJCWfJf7QrvZSfMaAmq6MWpbeGs```


## 3. Build and Run (Docker)
```docker build -f ./Dockfile/Dockerfile -t k4security/kschain-resolver .```
```docker run -p 8080:8080 k4security/kschain-resolver```

## 4. Example request
```curl -X GET http://localhost:8080/1.0/identifiers/did:kscirc:k12NqvVM9BX6AaMjPK1hUTUkKBWPBAUXAszTxdx7jDZPv4iqCZ1D```
```curl -X GET http://localhost:8080/1.0/identifiers/did:kscirc:k17qQYbApdfTdxsrS77k3sbFmJCWfJf7QrvZSfMaAmq6MWpbeGs```

