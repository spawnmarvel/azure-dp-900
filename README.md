# Microsoft Certified: Azure Data Fundamentals

## azure dp-900

https://learn.microsoft.com/en-us/credentials/certifications/azure-data-fundamentals/?practice-assessment-type=certification&source=learn

## Practice Assessments for Microsoft Certifications

https://learn.microsoft.com/en-us/credentials/certifications/practice-assessments-for-microsoft-certifications

Above 90

## 1 Microsoft Azure Data Fundamentals: Explore core data concepts

### Explore core data concepts

Introduction

Identify data formats

Structured data

* Structured data is often stored in a database in which multiple tables can reference one another by using key values in a relational model
* rdbms

Semi-structured data

* Semi-structured data is information that has some structure, but which allows for some variation between entity instances. For example, while most customers may have an email address, some might have multiple email addresses, and some might have none at all.
* json

Unstructured data

* Not all data is structured or even semi-structured. For example, documents, images, audio and video data, and binary files might not have a specific structure.

Data stores (There are two broad categories of data store in common use:)

* File stores
* Databases

Explore file storage

* Local HD, usb or shared file storage system

Delimited text files

* Data is often stored in plain text format with specific field delimiters and row terminators. The most common format for delimited data is comma-separated values (CSV) in which fields are separated by commas, and rows are terminated by a carriage return / new line.

```csv
FirstName,LastName,Email
Joe,Jones,joe@litware.com
Samir,Nadoy,samir@northwind.com

```

JavaScript Object Notation (JSON)

```json
{
  "customers":
  [
    {
      "firstName": "Joe",
      "lastName": "Jones",
      "contact":
      [
        {
          "type": "home",
          "number": "555 123-1234"
        },
        {
          "type": "email",
          "address": "joe@litware.com"
        }
      ]
    },
    {
      "firstName": "Samir",
      "lastName": "Nadoy",
      "contact":
      [
        {
          "type": "email",
          "address": "samir@northwind.com"
        }
      ]
    }
  ]
}

```

Extensible Markup Language (XML)

```xml
<Customers>
  <Customer name="Joe" lastName="Jones">
    <ContactDetails>
      <Contact type="home" number="555 123-1234"/>
      <Contact type="email" address="joe@litware.com"/>
    </ContactDetails>
  </Customer>
  <Customer name="Samir" lastName="Nadoy">
    <ContactDetails>
      <Contact type="email" address="samir@northwind.com"/>
    </ContactDetails>
  </Customer>
</Customers>

```

Binary Large Object (BLOB)

* Common types of data stored as binary include images, video, audio, and application-specific documents.


Optimized file formats

While human-readable formats for structured and semi-structured data can be useful, they're typically not optimized for storage space or processing.

Avro

* Row-based format. It was created by Apache. Each record contains a header that describes the structure of the data in the record. This header is stored as JSON. The data is stored as binary information.
* Is a good format for compressing data and minimizing storage and network bandwidth requirements.

ORC

* ORC (Optimized Row Columnar format) organizes data into columns rather than rows. 
* It was developed by HortonWorks for optimizing read and write operations in Apache Hive (Hive is a data warehouse system that supports fast data summarization and querying over large datasets). An ORC file contains stripes of data.

Parquet

* Parquet is another columnar data format. It was created by Cloudera and X. A Parquet file contains row groups. 
* Data for each column is stored together in the same row group. Each row group contains one or more chunks of data. 
* A Parquet file includes metadata that describes the set of rows found in each chunk. 
* An application can use this metadata to quickly locate the correct chunk for a given set of rows, and retrieve the data in the specified columns for these rows. Parquet specializes in storing and processing nested data types efficiently. It supports very efficient compression and encoding schemes.



Explore databases

Explore transactional data processing

Explore analytical data processing

Knowledge check


### Explore data roles and service

## 2 Microsoft Azure Data Fundamentals: Explore relational data in Azure

### Explore fundamental relational data concepts

### Explore relational database services in Azure

## 3 Microsoft Azure Data Fundamentals: Explore non-relational data in Azure

### Explore Azure Storage for non-relational data

### Explore fundamentals of Azure Cosmos DB

## 3 Microsoft Azure Data Fundamentals: Explore data analytics in Azure

### Explore fundamentals of large-scale analytics

### Explore fundamentals of real-time analytics

### Explore fundamentals of data visualization

