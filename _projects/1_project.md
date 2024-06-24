---
layout: page
title: HIS-ELK
description: The HIS-ELK project is designed to automatically monitor Hospital Information System (HIS) services and server statuses.
img: assets/img/project/HIS.jpg
importance: 1
category: work
related_publications: false
giscus_comments: true
---

The HIS-ELK project is designed to automatically monitor Hospital Information System (HIS) services and server statuses. By integrating the ELK (Elasticsearch, Logstash, Kibana) stack, this system streamlines data retrieval and visualization, facilitating efficient monitoring and analysis of HIS performance and issues.

## Table of Contents

- [ELK introduction](#elk-introduction)
- [HIS-ELK System Structure](#his-elk-system-structure)
- [Features](#features)
- [Reference](#reference)

## ELK introduction

The ELK stack, consisting of Elasticsearch, Logstash, and Kibana, is a powerful solution for real-time data analysis and visualization.

- Elasticsearch: A distributed search and analytics engine for storing and indexing data.
- Logstash: A data processing pipeline that ingests, transforms, and sends data to Elasticsearch.
- Kibana: A visualization tool for exploring and interacting with data stored in Elasticsearch.

Together, they enable comprehensive log and event data analysis, making it easier to monitor applications, troubleshoot issues, and gain insights. The ELK stack is scalable, flexible, and widely used for its powerful capabilities in handling large volumes of data efficiently.

This is a sort ppt for introduction [PPT](https://gamma.app/docs/HIS-ELK-4q9fkxld3pgwf9w).

## HIS-ELK System Structure

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="/assets/img/project/HIS_ELK.drawio.png" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

## Features

- **Automated Data Requests:** Periodically requests data from the ELK stack.
- **Data Processing:** Cleans and processes the data for analysis.
- **Visualization:** Generates visual reports and dashboards using Kibana.
- **Scheduling:** Automates the report generation process on a weekly basis.

## Reference

This project is based on this blog [Elastic blog post](https://www.elastic.co/blog/getting-started-with-the-elastic-stack-and-docker-compose-part-2).
