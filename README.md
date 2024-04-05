# TeamTechTitans-Katas2024

Team TechTitans Architectural Katas by O'Reilly, April 2024

## Team Members:
- [***Manas Chaturvedi***](https://www.linkedin.com/in/manaschaturvedi2202/)
- [***Saransh Jain***](https://www.linkedin.com/in/saranshj9/)
- [***Shishir Kumar***](https://www.linkedin.com/in/shishir1995/)
- [***Greeva Shah***](https://www.linkedin.com/in/greevashah/)
- [***Sumeet Singh***](https://www.linkedin.com/in/sumeet-singh-724839133/)

---

# Fish Watch

## Business Context
Livestock Insights Incorporated is a company headquartered in Scotland, but
operating globally.

Their main service offering, Fishy Watch, is used by Fish Farmers around the world to monitor their fish, and the fish farms in general
It is able to collect information about individual fish, water quality, and weather information.

Fish farmers use this information to understand the health of their livestock, check for signs of parasites and disease, and work out the best time to harvest.

## Business Requirements
| # | Description |
| ---- |-------------|
| BR1      | Customer Farm Management <br> - Customers may operate multiple fish farms in various geographical locations. <br> - Farms are divided into enclosures where fish are kept, ranging from a few to over a thousand enclosures per farm. <br> - Each enclosure is equipped with water monitors capturing data on pH, temperature, salinity, oxygen levels, and other factors. <br> - Underwater cameras provide general insights into fish health, monitoring size, activity, and parasite detection. |
| BR2      | Individual Fish Monitoring <br> - A beta feature allows individual fish identification through fish-ual recognition for health and lifecycle monitoring. |
| BR3 | Dashboard Customization <br> - Farmers require customizable dashboards to view collected information. |
| BR4 | Threshold-based Timely Alerts <br> - Farmers need to set thresholds for receiving alerts, ranging from basic parameters like pH levels to advanced warnings for adverse weather events. |
| BR5 | Data Aggregation <br> - Raw Data from multiple hardwares in multiple fish enclosures should be utilized to develop models predicting factors contributing to successful harvests. |
| BR6 | Multi-species Support <br> - Farms may host various fish species. |
| BR7 | Worldwide Insights <br> - Large customers seek insights across multiple farms and multiple geographies. |
| BR8 | Continuous Improvement <br> - Expectation for a similar system for other livestock like cattles and support for new hardware devices. |

## Technical Requirements
| # | Description |
| ---- |-------------|
| TR1      | Connectivity in Remote Areas <br> - Considerations for remote fish farm locations with poor cellular signal. |
| TR2      | Data Transmission <br> - Define mechanisms for hardware devices to transmit collected data to the system. |
| TR3 | Device Accessibility <br> - Fish Watch should be accessible from various devices, including rugged industrial devices used at sea during harvest. |
| TR4 | Future Scalability <br> - Architect the system to accommodate potential expansion into cattle monitoring and aquarium health management. |

## Target Audience

- **Fish Farmers**: Primarily, fish farmers who operate fish farms of various sizes and may have multiple farms in different geographical locations. Who may find this system useful for monitoring fish health and behavior.

- **Decision-makers and Executives**: Industrialists who own organization which have tie ups with multiple farm owners. They are responsible for making strategic decisions for large-scale industry wide farming operations.

- **Data Scientists and Analysts**: Professionals who analyze the collected data to derive insights and develop models for predicting factors contributing to successful harvests.
   
- **Researchers**: Professionals engaged in research related to aquaculture, fish health, and behavior.

- **Livestock Insights Inc. Support and Developers**: Individuals responsible for managing, maintaining, and developing the Fish Watch system, including its software, hardware, and data infrastructure.

- **Regulatory Authorities**: Regulatory agencies overseeing aquaculture/livestock practices, who may use the system to monitor compliance and ensure the health and welfare of farmed fish.

## High Level Architecture
Below is the proposed high level architecture for implementing the FishWatch solution:

![High Level Architecture](Assets/high-level-diagram.png)

## Architecture Characteristics

![Architecture Characteristics Worksheet](Assets/architecture-worksheet.png)

| Architecture Characteristics  | Business Needs |
| ------------- | ------------- |
| Responsiveness | ***Fishy Watch*** must swiftly provide real-time data to farmers, ensuring they can promptly respond to any changes in fish health, water quality, or environmental conditions, thus optimizing farm management practices. |
| Performance | It should efficiently process and analyze large volumes of data collected from multiple farms and devices, ensuring that farmers can access insights without experiencing delays or performance issues. |
| Availability | Ensure uninterrupted access to ***Fishy Watch*** regardless of their location or connectivity constraints. |
| Concurrency  | Support multiple farmers accessing and updating data concurrently without conflicts or inconsistencies, ensuring that each user's actions are accurately reflected in the system in real-time. |
| Data Integrity | Maintain the accuracy, consistency, and reliability of data throughout its lifecycle, implementing measures to prevent data corruption, unauthorized modifications, or loss, thereby ensuring the trustworthiness of the information available to farmers. |
| Security  | Protect sensitive farm data from unauthorized access, breaches, or cyber threats through robust authentication, encryption, and access control mechanisms, safeguarding the confidentiality, integrity, and availability of the data. |
| Scalability | Design the system to seamlessly accommodate the increasing data loads, user demands, and business growth, ensuring that it can scale horizontally or vertically to meet evolving requirements without compromising performance or reliability. |

## Architecture Style Decisions
[Architectural Approach](ADRs/000-architectural-approach.md)
![Architecture Styles Worksheet](Assets/architecture-styles-worksheet.png)
