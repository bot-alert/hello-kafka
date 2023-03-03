# Hello-Kafka

Hello-Kafka is a simple application that receives requests from `/api/v1/message` and publishes them to a Kafka topic. It also has an active listener that listens to the published topic and prints the message to the console.

## Prerequisites

Before you can run this application, you'll need to have the following installed:

- Java (version X or higher)
- Apache Kafka (version X or higher)

## Getting Started

To get started with Hello-Kafka, follow these steps:

1. Clone this repository to your local machine.
2. Configure the Kafka topic, producer, and consumer settings in the `application.properties` file.
3. Build the project using Maven: `mvn clean package`
4. Run the application using the Spring Boot Maven plugin: `mvn spring-boot:run`
5. Send a POST request to `localhost:8080/api/v1/message` with a message in the request body.
6. Check the console to see the message that was received by the Kafka listener.

## Configuration

The following configuration files are available in the project:

- `KafkaTopicConfig.java`: Configures the Kafka topic settings.
- `KafkaProducerConfig.java`: Configures the Kafka producer settings.
- `KafkaConsumerConfig.java`: Configures the Kafka consumer settings.

## Contributing

If you'd like to contribute to Hello-Kafka, please follow these guidelines:

1. Fork this repository.
2. Create a new branch for your changes.
3. Make your changes and commit them to your branch.
4. Push your branch to your forked repository.
5. Create a pull request from your branch to this repository's `README.md` file.

We appreciate your contributions and will review your pull request as soon as possible!

## License

Hello-Kafka is released under the MIT License. See `LICENSE` file for details.
