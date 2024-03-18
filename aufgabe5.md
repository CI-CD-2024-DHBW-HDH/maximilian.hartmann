# Aufgabe 5

## Welche Vorteile hat Kubernetes Deployment gegenüber einem Kubernetes Pod?
 - Möglichkeit zur Skalierung
 - automatisches lifecycle management der beinhalteten pods
 - Failende Pods werden in deployments automatisch ersetzt um den vorgegebenen State zu erhalten
 - zentrale Verwaltung/Updates der definierten Pods

## Wofür ist ein Kubernetes Service gut?
- ein Service macht einen definierten Port eines Pods innerhalb des Kubernetes Cluster für andere Pods erreichbar
- kann Load balancing übernehmen
- kann über NodePort die Pods von außerhalb erreichbar machen

## Wege, wie man eine Kubernetes Anwendung von außen erreichen kann:
- Cluster IP: Die Anwendung wird auf einer internen IP Adresse innerhalb des Clusters bereitgestellt
- NodePort: Bildet interne IP und Portnummer auf einem externen Port ab. Auf jedem Knoten eines Clusters wird dieser gleiche Port konfiguriert und leitet ankommende Anfragen an die Pods weiter
- LoadBalancer: Erstellt externen Load Balancer
- Ingress-Controller