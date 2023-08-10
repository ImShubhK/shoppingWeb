# shoppingWeb

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Java Development Kit (JDK)
- [Gradle](https://gradle.org/install/)
- Access to a PostgreSQL Database

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/shoppingWeb.git
2. Navigate to the project directory:
3. Initialize Gradle project:
       gradle init
4. Edit the build.gradle file and add the PostgreSQL JDBC driver dependency:

   dependencies {
    
    implementation 'org.postgresql:postgresql:<version>'
}
5.Modify the Java code in your project to establish a connection to your PostgreSQL database using the JDBC driver. Example code for database connectivity:

      spring.datasource.url = jdbc:postgresql://localhost:5432/web_application
      spring.datasource.username = <your username>
      spring.datasource.password =<password>
      spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
      spring.jpa.hibernate.ddl-auto=update

6.  Build and run your project:
              radle run

This project is licensed under the MIT License.
