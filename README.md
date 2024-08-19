Here's a `README.md` file for your `weather-app` project:

```markdown
# Weather App

The Weather App is a simple web application built with Spring Boot that allows users to retrieve and display current weather information for a specified city. The app consumes data from the OpenWeatherMap API and presents it in a user-friendly format.

## Features

- **City-based Weather Search:** Enter the name of a city to get the current weather details.
- **Weather Details:** Displays temperature, humidity, wind speed, weather description, and an icon representing the current weather.
- **Responsive Design:** The application is designed to be accessible on various screen sizes.

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- Java 8 or later
- Maven
- An API key from [OpenWeatherMap](https://openweathermap.org/api)

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/harshal-rembhotkar/weather-app.git
   cd weather-app
   ```

2. **Add your OpenWeatherMap API key:**

   In the `src/main/resources/application.properties` file, add your API key:

   ```properties
   api.key=your_openweathermap_api_key
   ```

3. **Build the project:**

   Use Maven to build the project:

   ```bash
   mvn clean install
   ```

4. **Run the application:**

   ```bash
   mvn spring-boot:run
   ```

5. **Access the application:**

   Open your web browser and go to `http://localhost:8080`.

## Usage

- **Home Page:** The home page is accessible at `/` and provides a form to enter the city name.
- **Weather Page:** After submitting the form, the weather details for the specified city will be displayed on the `/weather` page.

## Project Structure

- **Controller:** Handles HTTP requests and serves the appropriate views.
  - `WeatherController`: Manages weather-related requests and responses.
  
- **Model:** Represents the data structures used in the application.
  - `WeatherResponse`: Contains nested classes (`Sys`, `Weather`, `Main`, `Wind`) to model the response from the OpenWeatherMap API.
  
- **Application:** The entry point of the Spring Boot application.
  - `WeatherAppApplication`: Bootstraps the Spring Boot application.


## Dependencies

- [Spring Boot](https://spring.io/projects/spring-boot) - A framework that simplifies the development of Java applications.
- [Thymeleaf](https://www.thymeleaf.org/) - A modern server-side Java template engine.
- [OpenWeatherMap API](https://openweathermap.org/api) - A service providing weather data.


#Weather API website link: https://openweathermap.org/api
