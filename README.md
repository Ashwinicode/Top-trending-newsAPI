This README provides an overview of the News API, a Java-based application built with Spring Boot. The API retrieves the top 5 trending news articles from a specified website and returns them in JSON format upon request.
Table of Contents

    Introduction
    Setup
    Usage
    Endpoints
    Response Format
    Contributing
    License

Introduction

The News API is developed to provide developers with a simple and efficient way to access trending news articles from a website. By utilizing Java and Spring Boot, the API offers robustness and flexibility for integrating news data into various applications.
Setup

To set up the News API on your local machine, follow these steps:

    Ensure you have Java JDK and Maven installed.

    Clone the repository:

    bash

git clone https://github.com/your-username/news-api.git

Navigate to the project directory:

bash

cd news-api

Build the project using Maven:

mvn clean install

Run the application:

bash

    java -jar target/news-api.jar

    The API will now be running locally on http://localhost:8080.

Usage

Once the API is up and running, you can make HTTP requests to retrieve trending news articles. You can use tools like cURL, Postman, or any programming language's HTTP client to interact with the API.
Endpoints

The News API provides the following endpoints:

    /news/trending: Retrieves the top 5 trending news articles.

Response Format

The response returned by the API endpoint /news/trending will be in JSON format and will contain the following fields for each news article:

    title: The title of the news article.
    description: A brief description of the news article.
    url: The URL link to the full article.
    publishedAt: The date and time when the article was published.
    source: The source of the news article.

Example response:

json

[
    {
        "title": "Example News Article 1",
        "description": "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
        "url": "https://example.com/article1",
        "publishedAt": "2024-02-08T12:00:00Z",
        "source": "Example News"
    },
    {
        "title": "Example News Article 2",
        "description": "Nulla facilisi. Mauris consectetur purus at urna pulvinar, a elementum enim ultrices.",
        "url": "https://example.com/article2",
        "publishedAt": "2024-02-08T11:30:00Z",
        "source": "Example News"
    },
    ...
]

Contributing

Contributions to the News API project are welcome! If you find any bugs, have feature requests, or want to contribute code, please submit a pull request or open an issue on the GitHub repository.
