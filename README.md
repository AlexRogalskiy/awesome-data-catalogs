


# Awesome Data Discovery and Observability [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)

This repository contains a curated list of awesome data data catalogs and observability platforms that help you discover, manage, and observe data in your organization. 

<br>

## Contents: Existing Data Discovery and Observability Solutions

| [OSS Data Catalogs](#opensource) | [ Proprietary Monocloud DCs](#monocloud)| [ Proprietary Obserability Tools](#observability) | [Other Proprietary DCs](#proprietary) |
|--------------------------|--------------------------------|---------------------------------|--------------------------------|
| [📙 Amundsen](#amundsen) |  [📒 Google DC](#google)       | [🔍 Monte Carlo](#montecarlo)  | [📕 Alation](#alation)         |
| [📙 DataHub](#datahub)   |  [📒 Azure DC](#azure)         | [🔍 Databand](#databand)       | [📕 Atlan](#atlan)             |
| [📙 Marquez](#marquez)   |                                | [🔍 Datafold](#datafold)       | [📕 Collibra](#collibra)       |
| [📙 Atlas](#atlas)       |                                | [🔍 Ataccama](#ataccama)       | [📕 Informatica](#informatica) |
| [📙 CKAN](#ckan)         |                                |                                | [📕Stemma](#stemma)             |
| [📙 Magda](#magda)       |                                |                                |                                 |

<br>

## High-Level Feature Comparision

| Tool | Specification -Based | Search-based | Network-based | Lineage-based | Federa- tion | ML 1st Citizen | Data Quality | End-to-end Lineage | Observ- ability |
|:-------------:|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:| 
| [Alation](#alation)    | ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ |
| [Amundsen](#amundsen)  | ❌ | ✔️  | ✔️  | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌ |
| [Ataccama](#ataccama)  | ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ |
| [Atlan](#atlan)        | ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ |
| [Atlas](#atlas)        | ❌ | ✔️  | ❌  | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌|
| [Azure DC](#azure)     | ❌ | ✔️ | ? | ✔️ | ❌ | ❌ | ? | ❌ | ❌ |
| [CKAN](#ckan)          | ❌ | ✔️ | ❌  | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ |
| [Collibra](#collibra)  | ❌ | ✔️ | ?  | ✔️ | ❌ | ❌ | ? | ❌ | ❌ |
| [Databand](#databand)  | ❌ | ? | ? | ? | ❌ | ? | ? | ? | ✔️ |
| [Datafold](#datafold)  | ❌ | ✔️ | ✔️ | ✔️ | ❌ | ❌ | ✔️ | ❌ | ✔️ |
| [DataHub](#datahub)    | ❌ | ✔️  | ✔️ | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌ |
| [Google DC](#google)   | ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ | ? | ❌ | ❌ |
| [Informatica](#informatica)   | ❌ | ✔️ | ✔️  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ |
| [Magda](#magda)        | ❌ | ✔️ | ❌  | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ |
| [Marquez](#marquez)    | [OpenLineage](https://github.com/OpenLineage/OpenLineage) | ✔️ | ❌| ✔️ | ? | ❌ | ❌ | ❌ | ❌ |
| [Monte Carlo](#montecarlo)   | ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ | ✔️ | ❌ | ✔️ |
| [Stemma](#stemma)      | ❌ | ✔️ | ✔️  | ✔️ | ❌ | ❌ | ? | ❌ | ❌ |
| [Talend](#talend)      | ❌ | ✔️ | ? | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ |

Definitions:
<ul>
<li><b>Specification-based</b> - uses an open standard for collecting metadata to allow efficient time-to-discovery and federating data catalogs</li>
<li><b>Search-based</b> - allows to search for data assets</li>
<li><b>Lineage-based</b> - provides lineage for all entities the solution operates</li> 
<li><b>Network-based</b> - provides rich context about data asset ownership</li>
<li><b>Federation</b> - the ability to map multiple data catalogs into a single UI to avoid repeated data collection.</li> 
<li><b>End-to-end lineage</b> - data lineage that includes all data assets used in the organization across all its data catalogs and ML tools.</li> 
<li><b>ML 1st citizen</b> - operates ML entities on a high level - you can use them as any other data assets.</li> 
<li><b>Data Quality</b> - includes mature data quality assurance tools.</li> 
</ul>
<br>

<a name="opensource"></a>
## 📙 Open-Source Data Catalogs

<a name="amundsen"></a>
### Amundsen 
[Website](https://www.amundsen.io/) | [GitHub](https://github.com/amundsen-io/amundsen)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/amundsen-io/amundsen/graphs/commit-activity)
![](https://img.shields.io/github/stars/amundsen-io/amundsen.svg?style=social)

A popular open-source data catalog for metadata management and data discovery originated from Lyft. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ❌ | ✔️  | ✔️  | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b>  No</li> 
<li><b>Recommendations:</b> Yes </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> No </li>
<li><b>Data preview:</b> Yes </li>
<li><b>Column statistics:</b> Yes </li>
<li><b>Data owner:</b> Yes</li>
<li><b>Top data users:</b> Yes </li>
<li><b>Change notifications:</b>No </li>
<li><b>Change feed:</b> No </li>
<li><b>Deployment:</b>  </li> 
<li><b>Supported data sources:</b> Hive, Redshift, Druid, RDBMS, Presto, Snowflake </li>
</ul>
</details>

<br>

<a name="datahub"></a>
### DataHub

[Website](https://datahubproject.io/) | [GitHub](https://github.com/linkedin/datahub)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/linkedin/datahub/graphs/commit-activity)
![](https://img.shields.io/github/stars/linkedin/datahub.svg?style=social)

DataHub is an open-source data catalog featuring data discovery, data governance, metadata management originated from LinkedIn. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ❌ | ✔️  | ✔️ | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push, Pull</li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b> No</li> 
<li><b>Recommendations:</b> ? </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> No </li>
<li><b>Data preview:</b> ? </li>
<li><b>Column statistics:</b> No </li>
<li><b>Data owner:</b> Yes</li>
<li><b>Top data users:</b> ? </li>
<li><b>Change notifications:</b> No </li>
<li><b>Change feed:</b> No </li>
<li><b>Deployment:</b>  </li> 
<li><b>Supported data sources:</b> Hive, Kafka, RDBMS </li>
</ul>
</details>

<br>

<a name="marquez"></a>
### Marquez

[Website](https://marquezproject.github.io/marquez/) | [GitHub](https://github.com/MarquezProject/marquez)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/MarquezProject/marquez/graphs/commit-activity)
![](https://img.shields.io/github/stars/MarquezProject/marquez.svg?style=social)

Marquez is an open-source data catalog for collection, aggregation, and visualization of a data ecosystem’s metadata originated from WeWork. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:-----------:|:--:|:--:|:--:|:---:|:--:|:---:|:--:|:---:| 
| [OpenLineage](https://github.com/OpenLineage/OpenLineage) | ✔️ | ❌| ✔️ | ? | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b> No</li>
<li><b>Recommendations:</b> No </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> No </li>
<li><b>Data preview:</b> Yes </li>
<li><b>Column statistics:</b> No </li>
<li><b>Data owner:</b> Yes</li>
<li><b>Top data users:</b> ? </li>
<li><b>Change notifications:</b> No </li>
<li><b>Change feed:</b> No </li>
<li><b>Deployment:</b>  </li> 
<li><b>Supported data sources:</b> S3, Kafka </li>
</ul>
</details>

<br>

<a name="atlas"></a>
### Atlas 

[Website](https://atlas.apache.org/#/) | [GitHub](https://github.com/apache/atlas)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/apache/atlas/graphs/commit-activity)
![](https://img.shields.io/github/stars/apache/atlas.svg?style=social)

Apache Atlas is an open-source data catalog for metadata collection, governance, and data democratization.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ❌ | ✔️  | ❌  | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌|

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b> No</li>
<li><b>Recommendations:</b> No </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> No </li>
<li><b>Data preview:</b> No </li>
<li><b>Column statistics:</b> No </li>
<li><b>Data owner:</b> No</li>
<li><b>Top data users:</b> ? </li>
<li><b>Change notifications:</b> Yes </li>
<li><b>Change feed:</b> No </li>
<li><b>Deployment:</b>  </li>  
<li><b>Supported data sources:</b>HBase, Hive, Sqoop, Kafka, Storm  </li>
</ul>
</details>

<br>

<a name="ckan"></a>
### CKAN

[Website](https://ckan.org/) | [GitHub](https://github.com/ckan/ckan)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/ckan/ckan/graphs/commit-activity)
![](https://img.shields.io/github/stars/ckan/ckan.svg?style=social)

CKAN is an open-source data catalog for data management, powering data portals for govenments and enterprises. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ❌ | ✔️ | ❌  | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b> No</li>
<li><b>Recommendations:</b> ? </li>
<li><b>Schemas, Description:</b> ?</li>
<li><b>Complex schemas:</b> ? </li>
<li><b>Data preview:</b> ? </li>
<li><b>Column statistics:</b> ? </li>
<li><b>Data owner:</b> ?</li>
<li><b>Top data users:</b> ? </li>
<li><b>Change notifications:</b> ? </li>
<li><b>Change feed:</b> ? </li>
<li><b>Deployment:</b>  </li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="magda"></a>
### Magda

[Website](https://magda.io/) | [GitHub](https://github.com/magda-io/magda)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/magda-io/magda/graphs/commit-activity)
![](https://img.shields.io/github/stars/magda-io/magda.svg?style=social)

Magda is an open-source data catalog that features data discovery, metadata enrichment, and federation, focused on geodata.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ❌ | ✔️ | ❌  | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push via UI </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b> No</li>
<li><b>Recommendations:</b> No </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> No </li>
<li><b>Data preview:</b> Yes </li>
<li><b>Column statistics:</b> No </li>
<li><b>Data owner:</b> Yes</li>
<li><b>Top data users:</b> ? </li>
<li><b>Change notifications:</b> No </li>
<li><b>Change feed:</b> No </li>
<li><b>Deployment:</b>  </li> 
<li><b>Supported data sources:</b> Mostly geodata </li>
</ul>
</details>

<br>

<a name="proprietary"></a>
## 📕 Proprietary Data Catalogs

<a name="collibra"></a>
### Collibra

[Website](https://github.com/collibra) | [GitHub](https://github.com/collibra)

Collibra is an enterprise data catalog that helps to discover and understand data that matters and drive impactful insights from it.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:--:|:---:|:--:|:---:|:-:|:--:|:--:| 
| ❌ | ✔️ | ?  | ✔️ | ❌ | ❌ | ? | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> Yes</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="informatica"></a>
### Informatica

[Website](https://www.informatica.com/) | [GitHub](https://github.com/InformaticaCloudApplicationIntegration) 

Informatica is an enterprise data catalog that provides AI-powered data discovery engine to scan and catalog data assets. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:--:|:--:|:---:|:--:| 
| ❌ | ✔️ | ✔️  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> Yes</li> 
<li><b>Rich data profiling:</b> Yes</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

 <br>

<a name="alation"></a>
### Alation

[Website](https://www.alation.com/) | [GitHub](https://github.com/Alation)

Alation is a collaborative data catalog that helps companies to drive value and business impact from their data. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:--:|:--:|:---:|:---:| 
| ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> Yes</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> No</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="atlan"></a>
### Atlan

[Website](https://atlan.com/) | [GitHub](https://github.com/atlanhq)

Atlan is a modern data catalog offering data discovery, data profiling, data quality, data lineage and data governance.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:---:|:---:| 
| ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b> Presto, Deequ, Atlas, Airflow, Hudi  </li>
</ul>
</details>

<br>

<a name="stemma"></a>
### Stemma

[Website](https://www.stemma.ai/)  

Stemma is a fully managed data catalog powered by the open-source data catalog Amundsen that helps data teams have total trust in their data. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:| 
| ❌ | ✔️ | ✔️  | ✔️ | ❌ | ❌ | ? | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> No</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="talend"></a>
### Talend

[Website](https://www.talend.com/) | [GitHub](https://github.com/Talend)

Talend is a data catalog that helps enterprises power critical business descisions with trusted data. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:| 
| ❌ | ✔️ | ? | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> Yes</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> ?</li> 
<li><b>Rich data profiling:</b> Yes</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="monocloud"></a>
## 📒 Monocloud Data Catalogs

<a name="google"></a>
### Google Cloud Data Catalog

[Website](https://cloud.google.com/data-catalog) | [GitHub](https://github.com/GoogleCloudPlatform)

Google Cloud Data Catalog is a fully managed, scalable metadata management service in Google Cloud's Data Analytics family of products.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:| 
| ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ | ? | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> No</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="azure"></a>
### Azure Data Catalog

[Website](https://azure.microsoft.com/en-us/services/data-catalog/)  

Azure Data Catalog is a fully managed, enterprise-wide metadata catalog that makes data asset discovery straightforward.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:| 
| ❌ | ✔️ | ? | ✔️ | ❌ | ❌ | ? | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> ?</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="observability"></a>
## 🔍 Data Observability Platforms

<a name="montecarlo"></a>
### Monte Carlo

[Website](https://www.montecarlodata.com/)  

Monte Carlo is a data observability tool that helps to increase trust in data by eliminating or preventing data downtime.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:| 
| ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ | ✔️ | ❌ | ✔️ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> ?</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b> Snowflake, Hive, Kafka, Looker, Redshift, Tableau, Big Query, Airflow, Fivetran, Presto, Mode, Periscope, Databricks, Glue, dbt, Chartio, Spark, AWS, S3, data.world, Google Cloud Platform </li>
</ul>
</details>

<br>

<a name="databand"></a>
### Databand

[Website](https://databand.ai/) | [GitHub](https://github.com/databand-ai/)

Databand is an observability platform that helps data engineers identify and troubleshoot pipeline issues and data quality problems.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:| 
| ❌ | ? | ? | ? | ❌ | ? | ? | ? | ✔️ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> ?</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="datafold"></a>
### Datafold

[Website](https://www.datafold.com/) | [GitHub](https://github.com/datafold)

Datafold is a data monitoring and observability platform that gives you confidence in your data quality through diffs, profiling, and anomaly detection.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:| 
| ❌ | ✔️ | ✔️ | ✔️ | ❌ | ❌ | ✔️ | ❌ | ✔️ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> ?</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br> 

<a name="ataccama"></a>
### Ataccama

[Website](https://www.ataccama.com/) | [GitHub](https://github.com/ataccama)

Ataccama is an enterprise data catalog and observability tool featuring data profiling and data quality management, designed for data professionals.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:---:|:---:| 
| ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull </li>
<li><b>UX personalization:</b> Yes</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> Yes</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a href="#top">Back to top</a>
