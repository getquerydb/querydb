# QueryDB

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

QueryDB is a tool to allow anyone to take advantage of the power of large and small data, QueryDB allows connecting to multiple data sources, exploring and executing complex queries according to the language of the database engine, this data can be exported to many JSON, XML formats among others.

  - Connect Any Sources
  - Explore and Execue Complex query
  - Export Any Format

 QueryDB Features!

  - [Browser-based]: Everything in your browser
  - [Ease-of-use]: Become immediately productive with data widhout the need to master comlex software
  - [Query editor]: Quickly compose SQL an NoSQL querys with a schema browser and auto-complete
  - [REST API]: Everything that can be donde in the UI is also available through REST API
  - [Broad support for data sources]: extensible data source API with native support for a long list of common databases and platforms

### Getting started

You can run QueryDB in the following environments:

* [Application monolithic] - HTML enhanced for web apps!
* [Microservices] - awesome web-based text editor
* [Spring Cloud] - Markdown parser done right. Fast and easy to extend.

For production environments...

```sh
$ npm install --production
$ NODE_ENV=production node app
```

### Supported Data Sources

QueryDB supports more than 7 SQL and NoSQL datasources, it can also be extended to support more. Below is a lis of build-in sources.

Support Data Sources
- [x] MySQL
- [x] Oracle
- [x] SQL Server
- [x] PostgreSQL
- [x] Redis
- [x] Cassandra
- [x] Elasticsearch

#### Building for source
For production release:
```sh
$ mvn clean package --prod
```

### Docker
QueryDB is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the Dockerfile if necessary. When ready, simply use the Dockerfile to build the image.

```sh
docker build -t querydb/querydb:${package.json.version} .
```

Add the following dependency to your pom.xml after you have build this project locally.
```xml
<dependency>
	<groupId>com.querydb.querydb</groupId>
	<artifactId>querydb-cloud</artifactId>
	<version>1.0.0.RELEASE</version>
</dependency>
```

Create the Spring Cloud Dashboard with only one single Annotation.
```java
@SpringBootApplication
@EnableEurekaServer
@EnableDiscoveryClient
@EnableQueryDB
public class Application {
	public static void main(String[] args) {
		SpringApplication.run(Application.class, args);
	}
}
```
#### Reporting Bugs and Contributing Code
- Want to report a bug or request a feature? Please open [an issue.](https://github.com/getquerydb/querydb/issues/new)
- Want to help us build QueryDB? Fork the project, edit in a dev environment and make a pull request. We need all the help we can get!


### Security

Please email reyiclaros@gmail.com to report any security vulnerabilities. We will acknowledge receipt of your vulnerability and strive to send you regular updates about our progress

License
----

BSD-2-Clause.

