Panther Fuel

What is the proposed name for your Web application?
Panther Fuel
Who is the target audience for your Web application?
Student Athletes and coaches who are looking for better ways to find healthy food options.
What problem is it intended to solve for the target audience?
Student-Athletes have very busy schedules and struggle to find healthy food options eating out or healthy meals that they can prepare for the week. Pitt Athletics' Nurtritionist provides meal suggestions at restaurants, healthy recipes that the athletes can make and just general information on how to form their diet around their bust lifestyle. The website will allow them to create shopping carts based off of recipes the athletes choose so they can easily track what ingredients they need to buy. The website will also house restaurants in the area as well as common travel locations around the rest of the ACC. They will then be able to load recommended meal choices from these restaurants to better improve their diets.
How will it meet the minimum project requirements?
My site will be restricted to users with @pitt.edu email accounts only because its intended audience is Pitt's student-athletes. Once the user is logged in they will have access to all of the available content that has been provided by the nurtitionist. The nutritionist will have an admin panel to which he/she can login to update information and send new things to the website. All data will be accessed using RESTful services.
Why is your proposed Web application unique or creative beyond simply meeting the minimum requirements?
My application will have a real-world use. I work in Atheltics and our nutritionist has been looking to work on something like this and believes it was be very beneficial to Pitt's hundreds of student-athletes. It is a platform for her to make sure the student-athletes have access to every available resource to perform at the highest level.

## Build status


[![Build Status](https://travis-ci.org/infsci2560sp17/full-stack-web-stg34pitt.svg?branch=master)](https://travis-ci.org/infsci2560sp17/full-stack-web-stg34pitt)

## Web Site

[Seth's Website](https://secure-dawn-48368.herokuapp.com/)

## Key Features

TODO : Please list key features of your project.

* Key Feature 1
* Key Feature 2
* Key Feature N

## Project Details

### Landing Page

TODO : please provide a description of your landing page inluding a screen shot ![](https://.../image.JPG)

### User Input Form

TODO : please provide a description of at least 1 user input form including a screen shot ![](https://.../image.jpg)

## API

TODO : please provide a description of at least 1 API including a sample of request data and response data in both XML and JSON format.

### API Method 1

    POST photos/:id/tags

#### Parameters

- **id** _(required)_ — The Photo ID to add tags for.
- **tags** _(required)_ — Comma separated tags.

#### Response

A JSON or XMLobject containing the PhotoID and list of tags accepted.

#### Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'error' keys describing the source of error.

- **404 Not Found** — The photo was not found.

#### Example

##### Request

    POST /v1/photos/123456/tags

##### Body

    tags=cute,puppy


##### JSON Response

```json
{
    "photoId": 123456,
    "tags": ["cute", "puppy"]
}
```

##### XML Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<PhotoTags>
    <photoId>123456</PhotoId>
        <tags>
            <tag>cute</tag>
            <tag>puppy</tag>
        </tags>
</PhotoTags>
```

## Technologies Used

TODO : List all technologies used in your project

- [Spring Boot](https://projects.spring.io/spring-boot/) - Takes an opinionated view of building production-ready Spring applications.
- [Thymleaf](http://www.thymeleaf.org/) - Thymeleaf is a modern server-side Java template engine for both web and standalone environments.
- [Maven](https://maven.apache.org/) - Apache Maven is a software project management and comprehension tool.