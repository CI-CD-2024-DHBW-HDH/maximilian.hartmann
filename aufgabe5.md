# Aufgabe 5

## Welche Vorteile hat Kubernetes Deployment gegenüber einem Kubernetes Pod?
 - Möglichkeit zur Skalierung
 - automatisches lifecycle management der beinhalteten pods
 - Failende Pods werden in deployments automatisch ersetzt um den vorgegebenen State zu erhalten

## Wofür ist ein Kubernetes Service gut?
- ein Service macht einen definierten Port eines Pods innerhalb des Kubernetes Cluster für andere Pods erreichbar
- übernimmt Load balancing
- kann über NodePort die Pods von außerhalb erreichbar machen

## Wege, wie man eine Kubernetes Anwendung von außen erreichen kann:
- über Service (NodePort)
- ingress definieren