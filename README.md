![Databricks Badge](https://img.shields.io/badge/made%20with-Databricks-red)

## 🎉 Inspiration
We were struck by the lightning bolt ⚡ of inspiration when we discovered the incredible potential of Retrieval-Augmented Generation (RAG) and the mind-blowing scalability of Databricks. We thought, why not combine these two superpowers to create a RAG-based LLM model that can swoop in like a superhero 🦸‍♂️ and save the day for Husky's field service engineers? 

Company Website - [Husky Webpage](https://www.husky.co/en/)

About the Company - Husky Technologies specializes in [Injection Molding](https://en.wikipedia.org/wiki/Injection_moulding) systems and excels in providing top products and services for industries like consumer goods, medical, beverages, and automotive. They focus on delivering high-performance, efficient solutions globally, with extensive support including installation, training, and maintenance. Their commitment to innovation helps enhance productivity and profitability while fostering strong customer relationships.

Problem Statement - To enhance productivity for Husky Technologies' field service agents, implementing a Large Language Model (LLM) or a context-aware Q&A bot could be transformative. This technology would allow agents to quickly navigate complex documentation necessary for diagnosing equipment issues, significantly speeding up the process. The main challenge is integrating Husky's proprietary documents and internal knowledge into the LLM to ensure it can effectively retrieve and interpret specific information.

## 🤖 What it does
Our RAG-based LLM model is like a genius librarian 📚 that lives inside Databricks. It has memorized Husky's entire collection of technical documents and can provide spot-on answers to any question thrown its way. It's like having a pocket-sized expert 🧠 that engineers can consult anytime, anywhere!

## 🏛️ Architecture:

![alt text](https://github.com/ashwin975/Databricks_RAG/blob/main/Databricks_RAG.svg)

## 🛠️ How we built it
We donned our hard hats 👷‍♂️ and got to work, armed with Python and Databricks as our trusty tools. We used Elasticsearch as our retrieval sidekick 🔍, helping us find the most relevant passages in a flash. For the generative language model, we enlisted the help of the Hugging Face Transformers 🤗, training it to speak Husky's language. Databricks' distributed computing was the secret sauce 🌶️ that made everything run smoothly and efficiently.

## 😅 Challenges we ran into
Ensuring that the model's responses made sense and stayed on topic was like herding cats 🐱. Husky's documents are complex, and getting the retrieval process and model architecture just right took more trial and error than a mad scientist's lab 🧪. But we persevered, fueled by coffee ☕ and determination!

## 🎉 Accomplishments that we're proud of
We did it! We successfully combined the retrieval and generative components into a unified RAG model that provides accurate, context-specific answers. It's like we created a mind-reading machine 🔮 that can tap into Husky's collective knowledge and deliver coherent responses. We couldn't be prouder of our brainchild! 👶

## 🧠 What we learned
We learned that combining retrieval and generation techniques is like mixing peanut butter and jelly 🥪 - they're just meant to be together! We also discovered the importance of fine-tuning the retrieval process and optimizing the model architecture, like a chef perfecting a secret recipe 👨‍🍳. Databricks was our trusty sous-chef 👨‍🍳, handling the heavy lifting of data processing and model training.

## 🚀 What's next for RAG-based LLM on Databricks
The sky's the limit! 🌟 We plan to keep expanding the knowledge base, like a sponge soaking up water 🧽. We're also exploring ways to make the model handle multi-modal data, like a Swiss Army knife 🔧. Incorporating user feedback will be like having a built-in focus group 👥, helping us continuously improve. Integration with existing enterprise systems and support for multiple languages? That's like taking our model on a world tour 🌍! The future is bright, and we can't wait to see where this journey takes us! 🎈

## 🧅 Process Overview:
- Storage account, Databricks workspace, Databricks access connector, Resource group, Databricks metastore, cluster configurations were setup initially
- Connections and access management between Azure storage container and databricks workspace were established
- Ingestion and Transformations notebooks were created using SQL
- Workflow was orchestrated to run the notebooks sequentially

Key Benefits of Using Unity Catalog: 
- ✅ Build Efficient data flow layers ( raw -> processed -> presentation)
- ✅ Monitoring and Managing Pipelines with Azure Monitor service
- ✅ Setup up (CI/CD) pipelines to facilitate testing, deployment, and production phases
- ✅ Build Delta Lake in Azure databricks for ACID transactions
- ✅ Created External and Managed tables using Spark (PySpark and Spark SQL)
- ✅ Securely stored the secrets/credentials using Azure Key Vault
- ✅ Transformed the data using Azure Databricks for reporting and analysis
- ✅ Analyzed the data using Databricks and created Dashboards using Power BI
1. Data Discoverability: Data explorer provides a simple search through for any objects in catalog (with UI and SQL queries)
2. Data Audit: Audit logs/information can be viewed (when diagnostic settings are enabled)
3. Data Lineage: workflow, downstream and upstream datamovements can be viewed. With this we can perform root cause analysis, impact analysis and better manage data requiring regulatory compliance  
4. Data Access Control: Metastore access can be modified as required or as per user level (GRANT and REVOKE statements - SQL, CLI, also using Data Explorer)

## 🛠️ Tools Used:
 - Programming Language - SQL, PySpark, Python
 - Azure Cloud, Databricks
 - Azure Data lake Gen 2

## 🍽️ Dataset Used:
ERGAST API - Formula 1 Dataset - Drivers and Results JSON files
