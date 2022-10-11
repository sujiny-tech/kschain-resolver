<img src="https://user-images.githubusercontent.com/72974863/192973196-cb5b248b-d307-4fce-bae6-f3525681ea85.png" width=70% height=70%>

# Universal Resolver Driver: did:kscirc
This is a [Universal Resolver](https://github.com/decentralized-identity/universal-resolver/) driver for **did:kscirc** identifiers by K4-Security.   
This repository contains KSChian driver source code for DIF Unviversal Resolver. For the official KSChain DID Method specification, pleasae visit [the relative section](https://tangy-gallium-b9b.notion.site/DID-Method-Specification-KSChain-7a77664f1eae47769692f4ff2d029fe0).

## 1. Specification
### 1.1 KSChain DID Method Specification
+ [KSChain DID Method Specification](https://tangy-gallium-b9b.notion.site/DID-Method-Specification-KSChain-7a77664f1eae47769692f4ff2d029fe0)
### 1.2 Reference
+ [W3C DID Specification Registries](https://www.w3.org/TR/did-spec-registries/)
+ [W3C Decentralized Identifier v1.0](https://w3c.github.io/did-core/)
+ [W3C Decentralized Identifier Resolution v0.2](https://w3c-ccg.github.io/did-resolution/)


## 2. Example DIDs
```
did:kscirc:k12NqvVM9BX6AaMjPK1hUTUkKBWPBAUXAszTxdx7jDZPv4iqCZ1D    
did:kscirc:k17qQYbApdfTdxsrS77k3sbFmJCWfJf7QrvZSfMaAmq6MWpbeGs
```

## 3. Build and Run (Docker)
### 3.1 Pull kschain-resolver image from DockerHub
+ [DockerHub : KSChain-resolver](https://hub.docker.com/r/k4security/kschain-resolver)
```
docker pull k4security/kschain-resolver
docker run -p 8080:8080 k4security/kschain-resolver
```

## 4. Example request
### 4.1 curl test
```
curl -X GET http://localhost:8080/1.0/identifiers/did:kscirc:k12NqvVM9BX6AaMjPK1hUTUkKBWPBAUXAszTxdx7jDZPv4iqCZ1D    
curl -X GET http://localhost:8080/1.0/identifiers/did:kscirc:k17qQYbApdfTdxsrS77k3sbFmJCWfJf7QrvZSfMaAmq6MWpbeGs
```
## 5. Test Web page : DIF Universal Resolver
See https://dev.uniresolver.io/ for a DIF-hosted instance of the Universal Resolver that can be used for testing purposes.
