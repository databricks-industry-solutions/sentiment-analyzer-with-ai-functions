![image](https://raw.githubusercontent.com/databricks-industry-solutions/.github/main/profile/solacc_logo_wide.png)

![CLOUD](https://img.shields.io/badge/CLOUD-AWS+Azure-blue?logo=googlecloud&style=for-the-badge)
[![POC](https://img.shields.io/badge/POC-10_days-green?style=for-the-badge)](https://databricks.com/try-databricks)


# Sentiment Analysis With AI Functions

This Databricks Solution Accelerator provides a ready-to-use framework for analyzing customer sentiment in retail, leveraging in-built AI functions and foundation models in the Databricks Lakehouse Platform.

Understanding how customers feel about your brand and products is no longer a nice-to-have — it’s a competitive necessity. In a landscape where reviews, social media, and support interactions shape brand perception in real time, retailers must move beyond transactional data and tap into the voice of the customer.

This solution accelerator enables retail teams to analyze customer sentiment and product feedback at scale — using advanced analytics and machine learning to surface actionable insights. From detecting emerging product issues to uncovering sentiment trends by region, channel, or category, this solution helps brands get closer to their customers than ever before.

Retailers can use this accelerator to:
 - Extract and analyze sentiment from customer reviews, feedback, and social media
 - Identify trends in positive, neutral, and negative sentiment
 - Gain actionable insights to improve products, services, and customer experience
 - By embedding sentiment and feedback intelligence into core retail workflows, brands can respond faster, innovate smarter, and drive loyalty in an increasingly customer-driven world.

</p>
To assemble this application, *i.e.* the Sentiment Analyzer, we will need to obtain a series of documents that are relevant to the domain we wish to serve.  We will need to parse and store these to enable performant inference across the entire datasetset. We will then need to assemble the core analytical dashboards and natural language query space (Genie) which will allow our users to interact with the infered data.

We will tackle these three steps across a series of simple notebooks:</p>

- Load customer feedback data from Amazon
- Use out of the box AI functions in Databricks to deliver batch inference sentiment analysis on your data in only a few lines of cvode
- Create a single, simple pipeline to detect sentiment. This pipeline can then be used for managing tables for reporting, ad hoc queries, and/or decision support.
- Create a Genie room so you can explore your sentiment data with natural language interactions Create a dashboard for monitoring sentiment back to the business and drive insights and action
</p>
___
<mike.dobing@databricks.com>

---

&copy; 2025 Databricks, Inc. All rights reserved. The source in this notebook is provided subject to the Databricks License [https://databricks.com/db-license-source].  All included or referenced third party libraries are subject to the licenses set forth below.

| library                                | description             | license    | source                                              |
|----------------------------------------|-------------------------|------------|-----------------------------------------------------|
| datasets |This is a large-scale Amazon Reviews dataset, collected in 2023 by McAuley Lab| MIT  |   [https://pypi.org/project/langchain/](https://amazon-reviews-2023.github.io/main.html) |


## Getting started

Although specific solutions can be downloaded as .dbc archives from our websites, we recommend cloning these repositories onto your databricks environment. Not only will you get access to latest code, but you will be part of a community of experts driving industry best practices and re-usable solutions, influencing our respective industries. 

<img width="500" alt="add_repo" src="https://user-images.githubusercontent.com/4445837/177207338-65135b10-8ccc-4d17-be21-09416c861a76.png">

To start using a solution accelerator in Databricks simply follow these steps: 

1. Clone solution accelerator repository in Databricks using [Databricks Repos](https://www.databricks.com/product/repos)
2. Attach the `RUNME` notebook to any cluster and execute the notebook via Run-All. A multi-step-job describing the accelerator pipeline will be created, and the link will be provided. The job configuration is written in the RUNME notebook in json format. 
3. Execute the multi-step-job to see how the pipeline runs. 
4. You might want to modify the samples in the solution accelerator to your need, collaborate with other users and run the code samples against your own data. To do so start by changing the Git remote of your repository  to your organization’s repository vs using our samples repository (learn more). You can now commit and push code, collaborate with other users via Git and follow your organization’s processes for code development.

The cost associated with running the accelerator is the user's responsibility.


## Project support 

Please note the code in this project is provided for your exploration only, and are not formally supported by Databricks with Service Level Agreements (SLAs). They are provided AS-IS and we do not make any guarantees of any kind. Please do not submit a support ticket relating to any issues arising from the use of these projects. The source in this project is provided subject to the Databricks [License](./LICENSE). All included or referenced third party libraries are subject to the licenses set forth below.

Any issues discovered through the use of this project should be filed as GitHub Issues on the Repo. They will be reviewed as time permits, but there are no formal SLAs for support. 
---
