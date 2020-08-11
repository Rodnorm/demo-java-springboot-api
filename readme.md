# demo-java-springboot-api

First study with Java Springboot

##### How to run it

This project is built with Java 11. You should have it installed. If you do not, please download it from the official [source](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html).

* Download the repository
* Install the maven dependencies
* Click run 😄

##### Routes

So far I made only one which is:

```https:\localhost:{yourPortNumber}\api\v1\person
https:\localhost:{yourPortNumber}\api\v1\person
```

##### Model

This API stores a list of objects in the following model:

> {
>
> "name": "John Doe",
>
> "id": "aaa97d68-d64e-43ee-8be3-0aa0098916a1"
>
> }

##### Methods

GET:

* Returns all the persons registered on the database. If none is present, an empty array is returned.

POST:~~~~

* Sends a new Person object following the Person model in the body of the request in order to add a person to the database

PUT:

* Alter the data of an existing person. It takes a new Person as body and also the ID of the existing person as a url variable. Example below:


* Url

`https:\\localhost:{yourPortNumber}/api/v1/person/aaa97d68-d64e-43ee-8be3-0aa0098916a1`

* Body

```mermaid
{
    "name": "Joseph Doe",
    "id": "aaa97d68-d64e-43ee-8be3-0aa0098916a1"
}
```

DELETE:

* Removes one person given the matching of the ID of the person.
