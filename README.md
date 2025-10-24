# helm

## Übung 1.26 image ändern und kubectl einbauen 

```
alpine/k8s:1.31
```






## Übung 1.25 gitlab ci/cd 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/gitlab-ci-cd/example-helm-kubernetes.md
Schritt 1: Repo importieren 
-> Dieses Repo: https://gitlab.com/jmetzger/training-helm-chart-kubernetes-gitlab-ci-cd.git

## Übung 1.24 in gitlab einloggen 

## Übung 1.23 dependency with condition  - Exercise 2 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/dependencies/exercise.md#exercise-2-create-chart-with-condition

## Übung 1.22 dependency -Exercise 1 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/dependencies/exercise.md

## Übung 1.21 to yaml 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/exercises/01.01-TypeConversionToYaml-using-app-chart.md

## Übung 1.20 : Whitespace - Übung 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/templates/spaces.md

## Übung 1.19 : name templates verwenden

1) Wie sieht es aktuell im Namespace aus, wie heisst die pods

2) Name-templates app.labels und app.name verwenden
   && upgrade 

3) Welche Pods sind jetzt da, sind die alten Weg. 

## Übung 1.18 Ganz einfach starten 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/exercises/09-create-helm-chart-from-scratch-deployment.md

## Übung 1.17 nginx nach draussen lauschen lassen 

```
cd
mkdir helm-values
cd helm-values
mkdir my-app
cd my-app
```

```
nano values.yaml
```

```
service:
  type: LoadBalancer
```

```
cd
cd my-charts
helm -n my-app-jm upgrade --install my-app-release my-app --create-namespace --reset-values -f ../helm-values/my-app/values.yaml 

```

```
kubectl -n my-app-<namenskuerzel> get all
```

```
Im browser ip anzeigen
```



## Übung 1.16: Readiness - Check überprüft 

```
helm -n my-app-<namenskuerzel> get manifest my-app-release | less  
```

## Übung 1.15: Chart installieren 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/exercises/04a-create-chart-my-app-gruppenarbeit.md#install-helm---chart


## Übung 1.14: Eigenes Chart rendern 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/exercises/04a-create-chart-my-app-gruppenarbeit.md#chart-testen


## Übung 1.13. cloudpirates chart holen 

```
cd
helm pull oci://registry-1.docker.io/cloudpirates/mariadb --untar
```

## Übung 1.12 Eigenes Helm-Chart erstellen 

* nur 1. Punkt Chart erstellen 
https://github.com/jmetzger/training-helm-cicd/blob/main/helm/exercises/04a-create-chart-my-app-gruppenarbeit.md

## Übung 1.11 Umschauen get 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/exercises/install/mariadb-cloudpirates.md#umschauen-get

## Übung 1.10 Umschauen 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/exercises/install/mariadb-cloudpirates.md#umschauen

## Übung 1.9: helm exercises upgrade and values change 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/exercises/install/mariadb-cloudpirates.md#schritt-22-upgrade-und-resources-%C3%A4ndern

## Übung 1.8. Was kann ich konfigurieren (values) 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/exercises/install/mariadb-cloudpirates.md#schritt-21-default-values-auf-terminal-ausfindig-machen

## Übung 1.7 helm erkunden 

```
helm list
helm get <tab><tab>
helm get manifest my-mariadb
helm get manifest my-mariadb | less 
```



## Übung 1.6. helm exercises / mariadb 

https://github.com/jmetzger/training-helm-cicd/blob/main/helm/exercises/install/mariadb-cloudpirates.md#schritt-1-install-mariadb-von-cloudpirates

## Übung 1.5. deployment example 

https://github.com/jmetzger/training-kubernetes-einfuehrung/blob/main/kubectl-examples/03-nginx-deployment.md#example-deployment-nginx

## Übung 1.4. namespaces einrichten 

https://github.com/jmetzger/training-helm-cicd/blob/main/kubectl/kubectl-einrichten.md#arbeitsbereich-konfigurieren

## Übung 1.3. kubectl einrichten

  * https://github.com/jmetzger/training-helm-cicd/blob/main/kubectl/kubectl-einrichten.md

## Übung 1.2 ssh 

IP: 134.209.234.164
tln1 - trainer 
tln2 - Malvin 

## Übung 1.1 VPN 

https://vpn.newelements.de 
HELM-TR-43 - Trainer 

user: HELM-TN-01-43
pass: 
