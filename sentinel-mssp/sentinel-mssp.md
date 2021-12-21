# Microsoft Sentinel dans un contexte MSSP

*** DRAFT ***

<details><summary>Sommaire</summary>

* [Introduction](#intro)
* [Azure Lighthouse](#lighthouse)
* [Déploiement](#deployment)
* [Opérations](#operations)
* [Références](#references)

</details>

<a name="intro"></a>

## Introduction
Le [_Managed Security Service Provider_ (MSSP)](https://en.wikipedia.org/wiki/Managed_security_service), comme son nom l'indique, fournit des services de sécurité à ses clients.

Parmi ces services, celui qui nous intéresse est l'opération d'un [SOC (Security Operation Center)](https://en.wikipedia.org/wiki/Information_security_operations_center). Par ses fonctions de [SIEM et de SOAR](https://docs.microsoft.com/en-us/azure/sentinel/overview), [Microsoft Sentinel](https://azure.microsoft.com/services/azure-sentinel) est un bon candidat pour ce type de service. Comment s'y prendre en tant que fournisseur d'un service de SOC pour surveiller les environnements hybrides de ses clients, détecter et gérer les incidents de sécurité dans ces environnements, et déclencher les actions nécessaires ?

Cet article ne prétend pas être exhaustif sur le sujet puisque l'équipe CxE Sentinel a publié, début mars 2021, un guide complet sur le sujet : [Azure Sentinel Technical Playbook for MSSPs](https://aka.ms/azsentinelmssp), dont je recommande vivement la lecture préalable. Voir également [en fin d'article](#references) les autres sources qui font référence dans le domaine.

L'objectif de cet article est donc de fournir quelques éléments complémentaires et pratiques sur le sujet.

Pour utiliser Microsoft Sentinel dans un contexte où un MSSP fournit le service à plusieurs clients, il faut s'intéresser à :

 - Azure Lighthouse,
 - le déploiement automatisé de Microsoft Sentinel,
 - le fonctionnement de Microsoft Sentinel sur plusieurs tenants et plusieurs workspaces.

*** DRAFT ***

<a name="lighthouse"></a>

## Azure Lighthouse
*** DRAFT ***

<!--
Offres et délégations
Permissions nécessaires pour Sentinel
Exemple :
- Reader
- Microsoft Sentinel Contributor
- Log Analytics Reader

Cas particulier du CSP : comment donner au client des permissions pour qu'il puisse accéder aux données de Sentinel.
-->

<a name="deployment"></a>

## Déploiement
*** DRAFT ***

<!--
Automatisation du déploiement de Sentinel vers l'abonnement Azure du client
- Onboarding
- règles de détection
- requêtes de hunting
- playbooks
- workbooks
- connecteurs

PowerShell  
API  
ARM / Bicep

DevOps / CI/CD  
Azure DevOps / GitHub Actions
-->

<a name="operations"></a>

## Opérations
*** DRAFT ***

<!--
Ecrire des requêtes KQL multi-workspaces (à distance)  
Exemples CEF  
Utilisation de workspace()  
Utilisation de fonctions

Comment travailler depuis le workspace centralisé du MSSP  
Workbooks à distance  
Règles de détection à distance  
Règles avec requête planifiée

Autres règles  
Règles Fusion, Microsoft Security, ML Behavior Analytics  
La règle doit être dans le même workspace que les données  
Mais on peut attacher des actions (playbooks) dans un autre workspace (celui du MSSP)

=> Scripting de la mise en place des règles dans le workspace du client, avec Lighthouse.

-->

<a name="references"></a>

## Références

Document de référence :
- [Azure Sentinel Technical Playbook for MSSPs](https://aka.ms/azsentinelmssp) [pdf] (mars 2021)

Articles :
- [Build a scalable security practice with Azure Lighthouse and Azure Sentinel](https://azure.microsoft.com/en-us/blog/build-a-scalable-security-practice-with-azure-lighthouse-and-azure-sentinel/) (sept. 2020)
- [What’s New: Cross-workspace Analytics Rules](https://techcommunity.microsoft.com/t5/azure-sentinel/what-s-new-cross-workspace-analytics-rules/ba-p/1664211) (sept. 2020)
- [Protecting MSSP’s Intellectual Property in Azure Sentinel](https://techcommunity.microsoft.com/t5/azure-sentinel/protecting-mssp-s-intellectual-property-in-azure-sentinel/ba-p/1420941) (mai 2020)
- [Combining Azure Lighthouse with Sentinel’s DevOps capabilities](https://techcommunity.microsoft.com/t5/azure-sentinel/combining-azure-lighthouse-with-sentinel-s-devops-capabilities/ba-p/1210966) (mars 2020)

Documentation :
- [Azure Lighthouse: Manage Microsoft Sentinel workspaces at scale](https://docs.microsoft.com/en-us/azure/lighthouse/how-to/manage-sentinel-workspaces)
- [Extend Microsoft Sentinel across workspaces and tenants](https://docs.microsoft.com/en-us/azure/sentinel/extend-sentinel-across-workspaces-tenants)
- [Manage multiple tenants in Microsoft Sentinel as an MSSP](https://docs.microsoft.com/en-us/azure/sentinel/multiple-tenants-service-providers)
- [Protecting MSSP intellectual property in Microsoft Sentinel](https://docs.microsoft.com/en-us/azure/sentinel/mssp-protect-intellectual-property)

Autres liens utiles :
 - [Liens utiles sur Azure Lighthouse](https://aka.ms/lighthouse-links)
 - [Liens utiles sur Microsoft Sentinel](https://aka.ms/sentinel-links)

