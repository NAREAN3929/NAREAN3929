<h1 align="center">Narean Karthikeyan K</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=F59E0B&center=true&vCenter=true&width=620&lines=Software+Engineer+%7C+Data+Engineering;I+build+pipelines+that+move+data+reliably;Java+%C2%B7+SQL+%C2%B7+Spark+%C2%B7+Kafka+%C2%B7+Airflow" alt="Typing intro" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Location-Tamil%20Nadu%2C%20India-blue?style=flat-square" alt="Location" />
  <img src="https://komarev.com/ghpvc/?username=YOUR_USERNAME&style=flat-square&color=lightgrey&label=Profile+views" alt="Profile views" />
</p>

---

## About me

I'm a software engineer focused on **data engineering**. I design pipelines that collect, process, and deliver data at scale, from real-time event streams to scheduled batch jobs.

- Building: **[your current pipeline project]**
- Learning: **data modeling, Delta Lake / Iceberg, cloud data platforms, and data quality testing**
- Ask me about: **Kafka, Spark, Airflow, SQL tuning, and Java**

---

## How I think about data

```mermaid
flowchart LR
    A[Sources<br/>apps, APIs, logs] -->|events| B[(Kafka<br/>stream)]
    B --> C[Spark<br/>Structured Streaming]
    A -->|batch files| D[Spark<br/>batch jobs]
    C --> E[(Data lake)]
    D --> E
    E --> F[SQL<br/>warehouse models]
    F --> G[Dashboards<br/>and analytics]
    H{{Airflow<br/>orchestration}} -.schedules.-> D
    H -.monitors.-> F
```

---

## Tech stack

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL" />
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="Spark" />
  <img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white" alt="Kafka" />
  <img src="https://img.shields.io/badge/Apache%20Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white" alt="Airflow" />
</p>

| Layer | What I use it for |
| :-- | :-- |
| **Java** | Kafka producers and consumers, Spark applications, backend services |
| **SQL** | Window functions, CTEs, query tuning, dimensional modeling |
| **Apache Spark** | Batch ETL and Structured Streaming, partitioning and shuffle tuning |
| **Apache Kafka** | Event streaming, topics and partitions, consumer groups, exactly-once ideas |
| **Apache Airflow** | DAG scheduling, retries, backfills, SLAs and alerting |

---

## Featured projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>Real-time clickstream pipeline</h3>
      <b>Problem:</b> Website events arrive faster than batch reports can handle.<br />
      <b>Solution:</b> Kafka ingests events, Spark Streaming aggregates them in windows, results land in a SQL table.<br />
      <b>Result:</b> <i>[events per second, latency, e.g. "under 5 s end to end"]</i><br /><br />
      <img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" />
      <img src="https://img.shields.io/badge/Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" />
      <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" /><br /><br />
      <a href="https://github.com/YOUR_USERNAME/clickstream-pipeline">Code</a>
    </td>
    <td width="50%" valign="top">
      <h3>Daily batch ETL with Airflow</h3>
      <b>Problem:</b> Raw data needs cleaning and loading every night, with failures handled.<br />
      <b>Solution:</b> An Airflow DAG runs Spark jobs, validates the data, and loads warehouse tables.<br />
      <b>Result:</b> <i>[rows per run, runtime, e.g. "50M rows in 12 min"]</i><br /><br />
      <img src="https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white" />
      <img src="https://img.shields.io/badge/Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" />
      <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white" /><br /><br />
      <a href="https://github.com/YOUR_USERNAME/airflow-etl">Code</a>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Fraud detection stream</h3>
      <b>Problem:</b> Suspicious transactions need flagging in seconds, not hours.<br />
      <b>Solution:</b> Kafka transactions are scored by rules in Spark, alerts go to a separate topic.<br />
      <b>Result:</b> <i>[detection delay, accuracy on test data]</i><br /><br />
      <img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" />
      <img src="https://img.shields.io/badge/Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" /><br /><br />
      <a href="https://github.com/YOUR_USERNAME/fraud-stream">Code</a>
    </td>
    <td width="50%" valign="top">
      <h3>SQL optimization lab</h3>
      <b>Problem:</b> Slow queries hurt dashboards and costs.<br />
      <b>Solution:</b> A collection of before and after query rewrites with execution plan notes.<br />
      <b>Result:</b> <i>[e.g. "queries up to 20x faster"]</i><br /><br />
      <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white" /><br /><br />
      <a href="https://github.com/YOUR_USERNAME/sql-optimization-lab">Code</a>
    </td>
  </tr>
</table>

---

## Data engineering checklist I follow

- [x] Idempotent jobs, so reruns never create duplicates
- [x] Schema validation and data quality checks before loading
- [x] Retries, alerts, and backfill support in every DAG
- [x] Partitioning and file size tuned for Spark performance
- [x] Documented data flow for every pipeline

---

## GitHub stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=transparent&hide_border=true&title_color=F59E0B&icon_color=F59E0B" alt="GitHub stats" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_USERNAME&layout=compact&theme=transparent&hide_border=true&title_color=F59E0B" alt="Top languages" />
</p>

---

## Connect with me

<p align="center">
  <a href="mailto:narean3929@gmail.com" title="Gmail"><img src="https://img.shields.io/badge/-%20%20-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail" /></a>
  <a href="https://www.linkedin.com/in/narean3929" title="LinkedIn"><img src="https://img.shields.io/badge/-%20%20-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:narean3929@outlook.com" title="Outlook"><img src="https://img.shields.io/badge/-%20%20-0078D4?style=for-the-badge&logo=microsoftoutlook&logoColor=white" alt="Outlook" /></a>
  <a href="https://www.instagram.com/dheeran__narean" title="Instagram"><img src="https://img.shields.io/badge/-%20%20-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram" /></a>
</p>

---

<p align="center"><i>Good data is trusted data. Let's build pipelines people can rely on.</i></p>
