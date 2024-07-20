# Explore-end-to-end-analytics-with-Microsoft-Fabric
Microsoft Fabric is a unified data platform introduced by Microsoft to streamline and enhance data management and analytics capabilities across organizations. It integrates various data services and tools into a cohesive platform to support the entire data lifecycle, from ingestion and storage to transformation, analysis, and visualization.

Scalable analytics can be complex, fragmented, and expensive. With Microsoft Fabric, you don't have to spend all of your time combining various services from different vendors. Instead, you can use a single product that is easy to understand, set up, create, and manage. Fabric offers persona-optimized experiences and tools in an integrated user interface.

In addition to a simple, shared user experience, Fabric is a unified software-as-a-service (SaaS) offering, with all your data stored in a single open format in OneLake. OneLake is accessible by all of the analytics engines in the platform. Fabric offers scalability, cost-effectiveness, accessibility from anywhere with an internet connection, and continuous updates and maintenance provided by Microsoft.

###Explore OneLake
OneLake is Fabric's lake-centric architecture that provides a single, integrated environment for data professionals and the business to collaborate on data projects. Fabric's OneLake architecture facilitates collaboration between data team members and saves time by eliminating the need to move and copy data between different systems and teams. OneCopy is a key component of OneLake that allows you to read data from a single copy, without moving or duplicating data.

Think of it like OneDrive for data; OneLake combines storage locations across different regions and clouds into a single logical lake, without moving or duplicating data. Similar to how Office applications are prewired to use your organizational OneDrive, all the compute workloads in Fabric are preconfigured to work with OneLake. Fabric's data warehousing, data engineering (Lakehouses and Notebooks), data integration (pipelines and dataflows), real-time intelligence, and Power BI all use OneLake as their native store without needing any extra configuration.

![image](https://github.com/user-attachments/assets/1da6bfb8-c4f2-4f1c-b92a-ae6642d2b524)


OneLake is built on top of Azure Data Lake Storage (ADLS) and data can be stored in any format, including Delta, Parquet, CSV, JSON, and more.

What this means is that all of the compute engines in Fabric automatically store their data in OneLake. Data that is stored in OneLake is then directly accessible by all of the compute engines without needing to be moved or copied. For tabular data, the analytical engines in Fabric will write data in delta-parquet format and all engines interact with the format seamlessly.

One important feature of OneLake is the ability to create shortcuts, which are embedded references within OneLake that point to other files or storage locations. Shortcuts allow you to quickly source your existing cloud data without having to copy it, and enables Fabric experiences to derive data from the same source to always be in sync.

Screenshot of the OneLake architecture displaying the Delta-Parquet storage format as the foundation for serverless compute.
![image](https://github.com/user-attachments/assets/769bbc06-d055-468a-a1fc-8f2da20252fd)

Fabric offers a set of analytics experiences that are designed to accomplish specific tasks and work together seamlessly. Fabric's experiences include:

Synapse Data Engineering: data engineering with a Spark platform for data transformation at scale.
Synapse Data Warehouse: data warehousing with industry-leading SQL performance and scale to support data use.
Synapse Data Science: data science with Azure Machine Learning and Spark for model training and execution tracking in a scalable environment.
Synapse Real-Time intelligence: real-time intelligence to query and analyze large volumes of data in real-time.
Data Factory: data integration combining Power Query with the scale of Azure Data Factory to move and transform data.
Power BI: business intelligence for translating data to decisions.
Fabric provides a comprehensive data analytics solution by unifying all these experiences on a single platform.

###Explore security and governance
Fabric's OneLake is centrally governed and open for collaboration. Data is secured and governed in one place, while remaining discoverable and accessible to users who should have access across your organization. Fabric administration is centralized in the admin center.

In the admin center you can manage groups and permissions, configure data sources and gateways, and monitor usage and performance. You can also access the Fabric admin APIs and SDKs in the admin center, which you'd use to automate common tasks and integrate Fabric with other systems.

###Data teams and Microsoft Fabric

Microsoft Fabric's unified management and governance make it easier for data professionals to work together on data projects. Fabric removes data silos and the need for access to multiple systems, enhancing collaboration between data professionals.

Traditionally, the data engineer and data analyst role separation meant that there was an extra conversation that needed to happen to ensure that the engineer curated a perfect semantic model to help the analyst display data in an effective and insightful way for the business.

With Fabric, data professionals work together in the same SaaS product to better understand and identify needs of each other and the business. Further, data analysts now have greater context and ability to transform data further upstream with data factory.

Whether you're a data engineer looking to simplify your semantic model curation or expanding your knowledge with data science techniques, Fabric provides a complete experience to serve your organization.

For data analysts, who may have had to perform extensive downstream data transformations before creating Power BI reports, you can now see the lineage and connect with data more directly with DirectLake mode.

Data scientists now have an easier way to integrate native data science techniques and then use Power BI's interactive reporting to provide data-informed insights in a new way.

Because Fabric is a SaaS platform, it allows you to quickly and easily provision and run any type of workload or job without needing pre-approval or planning. This means that you can scale resources up or down as needed, and be more agile and responsive to changing business needs.

Lastly, Fabric is bringing the low-to-no-code concept, functionality, and approach that has successfully empowered many users on the Power Platform to its own SaaS offering. While it maintains scale and integrity for data science, data warehousing, data ingestion and prep, and analytics, it also offers many ways to visually represent code that previously blocked many from going further.

###Enable and use Microsoft Fabric

Before you can explore the end-to-end capabilities of Microsoft Fabric, it must be enabled for your organization. You may need to work with your IT department to enable Fabric for your organization. The permissions required to enable Fabric are either:

Fabric admin
Power Platform admin
Microsoft 365 admin
Fabric can be enabled at the tenant level or capacity level, meaning that it can be enabled for the entire organization or for specific groups of users. If you don't have access to Fabric, contact your Fabric administrator to find out if it's available to you. The Fabric administrator was formerly the Power BI administrator role.

###Enable Microsoft Fabric
If you have admin privileges, you can access the Admin center from the Settings menu in the upper right corner of the Power BI service. From here, you enable Fabric in the Tenant settings.

Admins can make Fabric available to either the entire organization or specific groups of users, who can be organized based on their Microsoft 365 or Microsoft Entra security groups. Admins can also delegate the ability to enable Fabric to other users, at the capacity level.

![image](https://github.com/user-attachments/assets/d1997604-59fc-4a99-b7e0-359e662f9c0c)

Note

If your organization isn't using Fabric or Power BI today, you can sign up for a free Fabric trial to explore the different workloads.

Create Fabric enabled workspaces
All Fabric items (lakehouses, notebooks, pipelines, etc.) are stored in OneLake and accessed via Fabric workspaces. To enable Fabric in a workspace, choose a Trial or Fabric Capacity license mode.

![image](https://github.com/user-attachments/assets/ba8a83a6-c3ec-40de-9cd2-17333306b14a)

Note

For more information on enabling Premium capacity in a workspace, see Fabric capacity settings.

###Create items in Fabric
After you create your Fabric enabled workspace, you can start creating items in Fabric. You can create items in Fabric using the Create menu in the upper left corner of the Power BI service.

![image](https://github.com/user-attachments/assets/f7bb084a-0eda-4e28-a698-8ac8133704c0)

###Explore Fabric workloads
Fabric workloads refer to the different capabilities included in Fabric. You can switch between workloads using the workload switcher in the bottom left corner of the navigation pane.

![image](https://github.com/user-attachments/assets/1ba8ac33-24d3-4fa4-a5e4-3e4de738e97a)


You may notice that Fabric workloads look similar to other Microsoft data offerings. Fabric is built on Power BI and Azure Data Lake Storage, and includes capabilities from Azure Synapse Analytics, Azure Data Factory, Azure Databricks, and Azure Machine Learning. What makes Fabric unique is that it brings these capabilities together in a single, SaaS integrated experience without the need for access to Azure resources.

