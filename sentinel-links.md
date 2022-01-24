# Microsoft Sentinel links

Quick link to this page: https://aka.ms/sentinel-links

<details><summary>Table of contents</summary>

* [General](#general)
* [Architecture](#architecture)
  * [General](#arch_general)
  * [Microsoft Sentinel for MSSPs](#mssp)
  * [Long term retention on Azure Data Explorer (ADX)](#adx)
* [Lab environments](#lab)
* [Data collection](#collection)
  * [Connectors reference](#connectors_reference)
  * [Azure Monitor Agent (AMA)](#ama)
  * [Microsoft 365 Defender integration](#m365d)
  * [SAP continuous threat monitoring](#sap)
* [Kusto query language (KQL)](#kql)
* [Advanced SIEM Information Model (ASIM)](#asim)
* [Notebooks and machine learning](#ml)
  * [Jupyter Notebooks](#notebooks)
  * [Bring your own Machine Learning (BYOML)](#byoml)
  * [Fusion ML detections](#fusion)
  * [User and Entity Behavior Analytics (UEBA)](#ueba)

</details>

<a name="general"></a>

## General
[Doc](https://docs.microsoft.com/en-us/azure/sentinel/) | [What’s new](https://aka.ms/asnew) | [Blog](https://aka.ms/microsoftsentinelblog) | [Discussion](https://techcommunity.microsoft.com/t5/microsoft-sentinel/bd-p/MicrosoftSentinel) | [GitHub](https://github.com/Azure/Azure-Sentinel) +[wiki](https://aka.ms/threathunters) | [Pricing](https://azure.microsoft.com/en-us/pricing/details/azure-sentinel/)  
[Security community](http://aka.ms/securitycommunity), [webinars](https://techcommunity.microsoft.com/t5/security-compliance-and-identity/recordings-security-community-webinars/ba-p/2865990)  
[Microsoft Sentinel Ninja Training](https://aka.ms/sentinelninja) +[FAQ](https://aka.ms/asfaq)

<a name="architecture"></a>

## Architecture

<a name="arch_general"></a>

### General
[Microsoft Sentinel workspace architecture best practices](https://docs.microsoft.com/en-us/azure/sentinel/best-practices-workspace-architecture)  
[Design your Microsoft Sentinel workspace architecture](https://docs.microsoft.com/en-us/azure/sentinel/design-your-workspace-architecture)  
[Azure Sentinel Deployment Guide (with Microsoft partner BlueVoyant)](https://azure.microsoft.com/en-us/resources/azure-sentinel-deployment-guide/)  
[Microsoft Cybersecurity Reference Architecture (MCRA)](https://aka.ms/mcra)

<a name="mssp"></a>

### Microsoft Sentinel for MSSPs

[Azure Sentinel Technical Playbook for MSSPs](https://aka.ms/azsentinelmssp) [pdf]  
[Extend Microsoft Sentinel across workspaces and tenants](https://docs.microsoft.com/en-us/azure/sentinel/extend-sentinel-across-workspaces-tenants)

How-to:
* [Manage multiple tenants in Microsoft Sentinel as an MSSP](https://docs.microsoft.com/en-us/azure/sentinel/multiple-tenants-service-providers)
* [Work with incidents in many workspaces at once](https://docs.microsoft.com/en-us/azure/sentinel/multiple-workspace-view)
* [Protecting MSSP intellectual property in Microsoft Sentinel](https://docs.microsoft.com/en-us/azure/sentinel/mssp-protect-intellectual-property)
* [Azure Monitor Logs for Service Providers](https://docs.microsoft.com/en-us/azure/azure-monitor/logs/service-providers)

[Azure Lighthouse: Manage Microsoft Sentinel workspaces at scale](https://docs.microsoft.com/en-us/azure/lighthouse/how-to/manage-sentinel-workspaces)

| date | webinar | video | deck |
| ---- | ------- | ----- | ---- |
| Apr 20, 2020 | MSSP and Distributed Organization Support | [YouTube](https://youtu.be/hwahlwgJPnE) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmgkkYuxOITkGSI7x8) |

2020-09-16 [Build a scalable security practice with Azure Lighthouse and Azure Sentinel](https://azure.microsoft.com/en-us/blog/build-a-scalable-security-practice-with-azure-lighthouse-and-azure-sentinel/)  
2020-09-14 [What’s New: Cross-workspace Analytics Rules](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/what-s-new-cross-workspace-analytics-rules/ba-p/1664211)  
2020-05-27 [Protecting MSSP’s Intellectual Property in Microsoft Sentinel](https://techcommunity.microsoft.com/t5/azure-sentinel/protecting-mssp-s-intellectual-property-in-azure-sentinel/ba-p/1420941)  
2020-03-05 [Combining Azure Lighthouse with Microsoft Sentinel’s DevOps capabilities](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/combining-azure-lighthouse-with-microsoft-sentinel-s-devops/ba-p/1210966)

<a name="adx"></a>

### Long term retention on Azure Data Explorer (ADX)

Doc : [Integrate Azure Data Explorer for long-term log retention](https://docs.microsoft.com/en-us/azure/sentinel/store-logs-in-azure-data-explorer)

| date | webinar | video | deck | blog |
| ---- | ------- | ----- | ---- | ---- |
| Mar 31, 2021 | Using Azure Data Explorer as Your Long Term Retention Platform of Azure Sentinel Logs | [YouTube](https://youtu.be/UO8zeTxgeVw) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmh0Nnt2bnuFtMWKOL?e=W0aiZ9) | [blog](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/using-azure-data-explorer-for-long-term-retention-of-microsoft/ba-p/1883947) |

2021-10-26 [Automation: Integrate Azure Data Explorer as Long-Term Log Retention for Microsoft Sentinel](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/automation-integrate-azure-data-explorer-as-long-term-log/ba-p/2512703)  
2021-04-28 [How to query data located in Azure Blob Storage, Azure Data Lake Store Gen2/1 with ADX](https://techcommunity.microsoft.com/t5/azure-data-explorer-blog/how-to-query-data-located-in-azure-blob-storage-azure-data-lake/ba-p/2301130)  
2021-04-13 [Azure Log Analytics Log Management using Azure Data Explorer](https://techcommunity.microsoft.com/t5/azure-data-explorer-blog/azure-log-analytics-log-management-using-azure-data-explorer/ba-p/2270478)

<a name="lab"></a>

## Lab environments
[Microsoft Sentinel To-Go](https://github.com/OTRF/Microsoft-Sentinel2Go)  
[Microsoft Sentinel Training Lab](https://github.com/Azure/Azure-Sentinel/tree/master/Solutions/Training/Azure-Sentinel-Training-Lab)  
2021-11-10 [Learning with the Microsoft Sentinel Training Lab](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/learning-with-the-microsoft-sentinel-training-lab/ba-p/2953403)

<a name="collection"></a>

## Data collection

<a name="connectors_reference"></a>

### Reference
[Data connectors reference](https://docs.microsoft.com/en-us/azure/sentinel/data-connectors-reference)

<a name="ama"></a>

### Azure Monitor Agent (AMA)
[Azure Monitor Agent (AMA)](https://docs.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-overview) and [Data Collection Rules (DCR)](https://docs.microsoft.com/en-us/azure/azure-monitor/agents/data-collection-rule-overview): [blog](https://techcommunity.microsoft.com/t5/azure-monitor-blog/a-powerful-agent-for-azure-monitor-and-a-simpler-world-of-data/ba-p/2443285)  
doc: [AMA-based connections](https://docs.microsoft.com/en-us/azure/sentinel/connect-azure-windows-microsoft-services?tabs=SA%2CAMA#windows-agent-based-connections)

[Webinars](https://techcommunity.microsoft.com/t5/security-compliance-and-identity/recordings-security-community-webinars/ba-p/2865990):

| date | webinar | video | deck |
| ---- | ------- | ----- | ---- |
| Nov 22, 2021 | Everything You Ever Wanted to Know About Using the New Azure Monitor Agent (AMA) with Microsoft Sentinel | [YouTube](https://youtu.be/Tvs-5JbGK-c) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmkVMcK42jaoKocz9Z?e=Itj8px) |

<a name="m365d"></a>

### Microsoft 365 Defender integration

[doc](https://docs.microsoft.com/en-us/azure/sentinel/microsoft-365-defender-sentinel-integration) | [how-to](https://docs.microsoft.com/en-us/azure/sentinel/connect-microsoft-365-defender)

2021-03-07 [Whats new: Azure Sentinel and Microsoft 365 Defender incident integration](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/whats-new-azure-sentinel-and-microsoft-365-defender-incident/ba-p/2191090)

<a name="sap"></a>

### SAP continuous threat monitoring
doc: [Deploy SAP continuous threat monitoring (preview)](https://docs.microsoft.com/en-us/azure/sentinel/sap-deploy-solution)

2021-12-11 [Microsoft Sentinel - SAP continuous threat monitoring workbooks](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/microsoft-sentinel-sap-continuous-threat-monitoring-workbooks/ba-p/3015630)  
2021-11-22 [Microsoft Sentinel - SAP continuous threat monitoring with UEBA entity pages](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/microsoft-sentinel-sap-continuous-threat-monitoring-with-ueba/ba-p/2981154)  
2021-05-19 [Protecting SAP applications with the new Azure Sentinel SAP threat monitoring solution](https://www.microsoft.com/security/blog/2021/05/19/protecting-sap-applications-with-the-new-azure-sentinel-sap-threat-monitoring-solution/)


[Webinars](https://techcommunity.microsoft.com/t5/security-compliance-and-identity/recordings-security-community-webinars/ba-p/2865990):

| date | webinar | video | deck |
| ---- | ------- | ----- | ---- |
| Nov 9, 2021 | SAP Mini-Series Part 2: Deep Dive - End-to-End Installation of SAP for Microsoft Sentinel | [YouTube](https://youtu.be/n8StWQ_jZbM) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmkVYkhX-N4UsnWmAJ?e=wGKYfP) |
| Oct 18, 2021 | SAP Mini-Series Part 1: Introduction to Monitoring SAP with Azure Sentinel for Security Professionals | [YouTube](https://www.youtube.com/watch?v=oG9GTc7g3Bg) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmjwkIAN5ljRtag3dh?e=s0iQQg) |

<a name="kql"></a>

## Kusto query language (KQL)
[KQL reference guide](https://docs.microsoft.com/en-us/azure/data-explorer/kusto/query/) | [Azure Monitor data reference](https://docs.microsoft.com/en-us/azure/azure-monitor/reference/)   
[Microsoft Sentinel Ninja Training](https://aka.ms/sentinelninja): part 3 modules 7 (KQL) & 8 (Analytics)  
Rod Trent's [Must Learn KQL - the Blog series](https://aka.ms/MustLearnKQL) | [Sample queries](https://github.com/rod-trent/SentinelKQL)  
Marcus Bakker's [KQL cheat sheet](https://github.com/marcusbakker/KQL?WT.mc_id=m365-0000-rotrent)  
[KQL lab Jupyter notebook](https://github.com/NorthwaveSecurity/azure_sentinel_learn_kql_lab)

| date | webinar | video | deck | blog/lab |
| ---- | ------- | ----- | ---- | -------- |
| Dec 7, 2021 | KQL Framework for Microsoft Sentinel -Empowering You to Become KQL-Savvy | [YouTube](https://youtu.be/j7BQvJ-Qx_k) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmkgqKSV-m1QWgkzKT?e=QAilwu) | [blog](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/advanced-kql-framework-workbook-empowering-you-to-become-kql/ba-p/3033766) |
| Sep 9, 2020 | KQL part 3 of 3 - Optimizing Azure Sentinel KQL queries performance | [YouTube](https://youtu.be/jN1Cz0JcLYU) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmg2imjIS8NABc26b-?e=rXZrR5) | |
| Jul 28, 2020 | KQL part 2 of 3: KQL hands-on lab exercises | [YouTube](https://youtu.be/YKD_OFLMpf8) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmhWSUcV-O-QIVxkAR) | |
| Jun 2, 2020 | KQL part 1 of 3: Learn the KQL you need for Azure Sentinel | [YouTube](https://youtu.be/EDCBLULjtCM) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmhWMvaCIya48sGVTL) | [lab](https://github.com/NorthwaveSecurity/azure_sentinel_learn_kql_lab/blob/master/azure_sentinel_learn_kql_lab.ipynb) |

2022-01-11 [Get Hands-On KQL Practice with this Microsoft Sentinel Workbook](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/get-hands-on-kql-practice-with-this-microsoft-sentinel-workbook/ba-p/3055600)  
2022-01-04 [Leveraging the Power of KQL in Incident Response](https://techcommunity.microsoft.com/t5/security-compliance-and-identity/leveraging-the-power-of-kql-in-incident-response/ba-p/3044795)

<a name="asim"></a>

## Advanced SIEM Information Model (ASIM)
(formerly *Azure Sentinel Information Model*)  
[Doc: Normalization and the Advanced SIEM Information Model (ASIM)](https://aka.ms/AzSentinelNormalization)  
[GitHub: Deploy ASIM parsers](https://github.com/Azure/Azure-Sentinel/tree/master/Parsers/ASim)  
2021-06-15 [What's new: Azure Sentinel Information Model DNS Schema and normalized content now public](https://techcommunity.microsoft.com/t5/azure-sentinel/what-s-new-azure-sentinel-information-model-dns-schema-and/ba-p/2429926)  
2021-07-01 [What's new: ASIM Authentication, Process, Registry and enhanced Network schemas](https://techcommunity.microsoft.com/t5/azure-sentinel/what-s-new-asim-authentication-process-registry-and-enhanced/ba-p/2502268)  
2021-08-04 [What's new: ASIM File Activity schema](https://techcommunity.microsoft.com/t5/azure-sentinel/what-s-new-asim-file-activity-schema/ba-p/2609732)

[Webinars](https://techcommunity.microsoft.com/t5/security-compliance-and-identity/recordings-security-community-webinars/ba-p/2865990):

| date | webinar | video | deck |
| ---- | ------- | ----- | ---- |
| Oct, 6, 2021 | Turbocharging ASIM: Making Sure Normalization Helps Performance Rather Than Impacting It | [YouTube](https://youtu.be/-dg_0NBIoak) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmjnQITNn35QafW5V2?e=GnCDkA) |
| Aug 11, 2021 | Deep Dive into Azure Sentinel Normalizing Parsers and Normalized Content | [YouTube](https://youtu.be/Yv1Ja0Sk6wY) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmjGtoRPQ2XYe3wQDz?e=R3dWeM) |
| Jul 28, 2021 | The Information Model: Understanding Normalization in Azure Sentinel | [YouTube](https://youtu.be/kTaKqQKzt_o) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmjDY1cro08Fk3KUj-?e=murYHG) |

<a name="ml"></a>

## Notebooks and machine learning

<a name="notebooks"></a>

### Jupyter Notebooks
[Doc](https://docs.microsoft.com/en-us/azure/sentinel/notebooks) | [GitHub](https://github.com/Azure/Azure-Sentinel-Notebooks)  
[Microsoft Sentinel Ninja Training](https://aka.ms/sentinelninja): part 3 module Y  
[Microsoft Sentinel Notebooks Ninja - The Series!](https://cda.ms/2wn)  
[Microsoft Sentinel Jupyter Notebooks knowledge check test](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/microsoft-sentinel-jupyter-notebooks-knowledge-check-test/ba-p/3030784)

[Webinars](https://techcommunity.microsoft.com/t5/security-compliance-and-identity/recordings-security-community-webinars/ba-p/2865990):

| date | webinar | video | deck | blog |
| ---- | ------- | ----- | ---- | ---- |
| Dec 16, 2021 | Become a Jupyter Notebooks Ninja – MSTICPy Fundamentals to Build Your Own Notebooks | [YouTube](https://youtu.be/S0knTOnA2Rk) |  |  |
| Oct 11, 2021 | Become a Notebooks Ninja – Getting Started with Jupyter Notebooks in Azure Sentinel | [YouTube](https://youtu.be/JLOhfoovASE) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmjmnUOdOAguEDWvz5?e=gYHOkU) |  |
| Jul 20, 2021 | Streamlining your SOC Workflow with Automated Notebooks | [YouTube](https://youtu.be/DinI1I1pbz4) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmi2wGTRPLKwedfnTg?e=Sei3an) | [blog](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/software-defined-monitoring-using-automated-notebooks-and-azure/ba-p/2587775) |
| Jul 13, 2021  | Customizing Azure Sentinel with Python - MSTICPy and Jupyter Notebooks | [YouTube](https://youtu.be/OC4TeNUxSR0) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmi1M7k3EWkflm-JYf?e=6ggEbr) |  |
| Jan 19, 2021 | Azure Notebooks Fundamentals – How to get started | [YouTube](https://youtu.be/rewdNeX6H94) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmhgtEKc1QwMM83p99) |  |

MSTICPy: [doc](https://msticpy.readthedocs.io/) | [GitHub](https://github.com/microsoft/msticpy) | [Medium](https://msticpy.medium.com/)

2022-01-13 [Single Sign On Support for authentication in Microsoft Sentinel Notebooks](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/single-sign-on-support-for-authentication-in-microsoft-sentinel/ba-p/3060112)  
2021-12-14 [Microsoft Sentinel Jupyter Notebooks knowledge check test](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/microsoft-sentinel-jupyter-notebooks-knowledge-check-test/ba-p/3030784)  
2021-11-02 [Security big data analytics with Azure Synapse and Microsoft Sentinel Notebooks!](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/security-big-data-analytics-with-azure-synapse-and-microsoft/ba-p/2916265)  
2021-06-01 [What’s new: Detect credential leaks using built-in Azure Sentinel notebooks!](https://techcommunity.microsoft.com/t5/azure-sentinel/what-s-new-detect-credential-leaks-using-built-in-azure-sentinel/ba-p/2406042)  
2021-05-21 [The Launch Space: Updates to MSTICPy and Jupyter Notebooks in Azure Sentinel](https://docs.microsoft.com/en-us/shows/The-Launch-Space/Updates-to-MSTICPy-and-Jupyter-Notebooks-in-Azure-Sentinel) | [YouTube](https://www.youtube.com/watch?v=m3YElHwZX1U)  
2021-04-26 [MSTICPy and Jupyter Notebooks in Azure Sentinel, an update](https://techcommunity.microsoft.com/t5/azure-sentinel/msticpy-and-jupyter-notebooks-in-azure-sentinel-an-update/ba-p/2279661)  
2021-04-19 [MSTICPy 1.0.0](https://msticpy.medium.com/msticpy-1-0-0-release-1e8848e45653)  
2021-01-29 [Jupyter Notebooks in VS Code](https://www.youtube.com/watch?v=g5EykzAsCC0&list=PLj6YeMhvp2S6uB23beQaffszlavLq3lNq&index=7)  
2020-11-18 [Using the VirusTotal V3 API with MSTICPy and Azure Sentinel](https://techcommunity.microsoft.com/t5/azure-sentinel/using-the-virustotal-v3-api-with-msticpy-and-azure-sentinel/ba-p/1893121)  
2019-04-22 [Why Use Jupyter for Security Investigations?](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/why-use-jupyter-for-security-investigations/ba-p/475729)

<a name="byoml"></a>

### Bring your own Machine Learning (BYOML)
[Doc](https://docs.microsoft.com/en-us/azure/sentinel/bring-your-own-ml) | [GitHub](https://github.com/Azure/Azure-Sentinel/tree/master/BYOML)  
2020-10-06 [Build-Your-Own Machine Learning detections in the AI immersed Azure Sentinel SIEM](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/build-your-own-machine-learning-detections-in-the-ai-immersed/ba-p/1750920)  
2020-10-09 [What's new: New Fusion detections and BYOML in public preview!](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/what-s-new-new-fusion-detections-and-byoml-in-public-preview/ba-p/1765990)  
2020-11-25 [Azure Sentinel | Build-Your-Own Machine Learning Model](https://techcommunity.microsoft.com/t5/microsoft-sentinel/azure-sentinel-build-your-own-machine-learning-model/m-p/1931792)

[Webinars](https://techcommunity.microsoft.com/t5/security-compliance-and-identity/recordings-security-community-webinars/ba-p/2865990):

| date | webinar | video | deck | blog |
| ---- | ------- | ----- | ---- | ---- |
| Jan 12, 2021 | Machine Learning detections in the AI-infused Azure Sentinel SIEM | [YouTube](https://youtu.be/DxZXHvq1jOs) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmhgUqL5UfmNuKNa81) | [blog](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/build-your-own-machine-learning-detections-in-the-ai-immersed/ba-p/1750920) |

<a name="fusion"></a>

### Fusion ML detections
Doc: https://aka.ms/SentinelFusion

[Webinars](https://techcommunity.microsoft.com/t5/security-compliance-and-identity/recordings-security-community-webinars/ba-p/2865990):

| date | webinar | video | deck | blog |
| ---- | ------- | ----- | ---- | ---- |
| Dec 1, 2021 | Fusion ML Detections for Emerging Threats & Configuration UI | [YouTube](https://youtu.be/bTDp41yMGdk) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmkW-CSAjk6o2O27Mx?e=fa0p2q) | [blog](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/detecting-emerging-threats-with-microsoft-sentinel-fusion/ba-p/2923835) |
| Aug 18, 2021 | Fusion ML Detections with Scheduled Analytics Rules | [YouTube](https://youtu.be/lmXHAAFBoPw) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmjQo_9QDdeDd1ufdj?e=HS3DAJ) | [blog](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/what-s-new-fusion-advanced-multistage-attack-detection-scenarios/ba-p/2337497) |

2021-11-04 [Detecting Emerging Threats with Microsoft Sentinel Fusion](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/detecting-emerging-threats-with-microsoft-sentinel-fusion/ba-p/2923835)  
2021-08-09 [What’s new: Fusion Detection for Ransomware](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/what-s-new-fusion-detection-for-ransomware/ba-p/2621373)  
2021-05-12 [What's New: Fusion Advanced Multistage Attack Detection Scenarios with Scheduled Analytics Rules](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/what-s-new-fusion-advanced-multistage-attack-detection-scenarios/ba-p/2337497)

<a name="ueba"></a>

### User and Entity Behavior Analytics (UEBA)

[Doc](https://docs.microsoft.com/en-us/azure/sentinel/identify-threats-with-entity-behavior-analytics)

| date | webinar | video | deck |
| ---- | ------- | ----- | ---- |
| 2022-01-19 | Present and Future of User Entity Behavioral Analytics in Microsoft Sentinel | [YouTube](https://youtu.be/dLVAkSLKLyQ) | [deck](https://1drv.ms/b/s!AnEPjr8tHcNmklCGjFh58XHq_tNO?e=WO8UNi) |