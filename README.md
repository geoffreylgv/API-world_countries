# world countries api

 [![GitHub license](https://img.shields.io/github/license/geoffreylgv/API-world_countries.svg)](https://github.com/geoffreylgv/API-world_countries/blob/main/LICENSE)
[![GitHub contributors](https://img.shields.io/github/contributors/geoffreylgv/API-world_countries.svg)](https://GitHub.com/geoffreylgv/API-world_countries/graphs/contributors/)
[![GitHub issues](https://img.shields.io/github/issues/geoffreylgv/API-world_countries.svg)](https://GitHub.com/geoffreylgv/API-world_countries/issues/)
[![GitHub pull-requests](https://img.shields.io/github/issues-pr/geoffreylgv/API-world_countries.svg)](https://GitHub.com/geoffreylgv/API-world_countries/pulls/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
![MIT Licence](https://img.shields.io/github/last-commit/geoffreylgv/API-world_countries)

[![GitHub watchers](https://img.shields.io/github/watchers/geoffreylgv/API-world_countries.svg?style=social&label=Watch)](https://GitHub.com/geoffreylgv/API-world_countries/watchers/)
[![GitHub forks](https://img.shields.io/github/forks/geoffreylgv/API-world_countries.svg?style=social&label=Fork)](https://GitHub.com/geoffreylgv/API-world_countries/network/)
[![GitHub stars](https://img.shields.io/github/stars/geoffreylgv/API-world_countries.svg?style=social&label=Star)]([https://GitHub.com/geoffreylgv/API-world_countries/stargazers/](https://img.shields.io/github/last-commit/geoffreylgv/API-world_countries))

## Running principal route for the api
```bash
  localhost:8090/country/api/v1
```
## Global Hack Week MLH : API Days contribution

**The API provides the following functionalities:**

##### Get a list of all countries:

` Request: GET /countries`

Response: A JSON array containing all the countries in the system, with their respective ID, code, name (in French and English), alpha2 and alpha3 codes.
##### Get a specific country by ID:

`Request: GET /countries/{id}`

Response: A JSON object containing the details of the country with the specified ID, including its code, name (in French and English), alpha2 and alpha3 codes.

##### Get a list of countries by name:

`Request: GET /countries?name={name}`

Response: A JSON array containing all the countries whose name (in French or English) contains the specified search term, along with their respective ID, code, name (in French and English), alpha2 and alpha3 codes.

##### Search for countries using any attribute:

`Request: GET /countries/search?q={query}`

Response: A JSON array containing all the countries who's any attribute contains the specified search term, along with their respective ID, code, name (in French and English), alpha2 and alpha3 codes.
The API is implemented using Spring Boot and utilizes the JPA/Hibernate framework for data persistence. The data model is represented by the "Country" entity, which is mapped to a database table called "COUNTRIES". The entity has the following attributes:

**Full Changelog**: https://github.com/geoffreylgv/API-world_countries/commits/v1.0.0

[<img src="https://i3.ytimg.com/vi/3M6ogLK_I-4/maxresdefault.jpg" width="100%">](https://www.youtube.com/watch?v=3M6ogLK_I-4 "Video on youtube, soon the API on Azure Functio APP")

id: A unique identifier for each country.<br>
code: A unique code assigned to each country.<br>
nameFR: The name of the country in French.<br>
nameEN: The name of the country in English.<br>
alpha2: The two-letter code assigned to each country.<br>
alpha3: The three-letter code assigned to each country.<br>

<quote>The entity also includes standard JPA annotations for defining the mapping to the database table and managing the persistence of the entity instances. The Lombok library is used to generate getters, setters, equals and hashcode methods for the entity class.</quote>

## How to use locally
1. Download the repos, 
2. make sure to update the application.propertie in resources folder 
3. make a clean and build and 
4. run <br>

>Insert country's data into countries table; that's all. With love, thanks you for reading. ^_^
