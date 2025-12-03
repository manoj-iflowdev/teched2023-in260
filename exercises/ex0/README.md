# Getting Started - Preparation

Before getting started with the exercise, let's check if you have all the prerequisites in place and understand the use case we intend to build an application for.

## Prerequisites

- Clone this repository to your local machine and open it using your preferred IDE.
  - We recommend using IntelliJ IDEA where you can select "File > New... > Project from Existing Sources" and select the cloned repository.
- (Optional) Log into your SAP BTP trial account. If you don't have one, you can create one at the SAP Developer portal.
  - This is only required if you would like to push your application to CloudFoundry.
  - However, all exercises can be completed locally without pushing to CloudFoundry.

<details> 
<summary>The necessary software for following the exercises is already installed on your systems.</summary>
If you want you could confirm the installations by running the following commands in your terminal:

- Java 17
   ```shell
      java -version
   ```
- Maven 3.9+

  ```shell 
     mvn -version
  ```
- Node 18+

  ```shell
     node --version
  ```
- Npm 9+

  ```shell
     npm --version
  ```
- cdsdk 7.0+

  ```shell
     cds --version
  ```
- cf cli 7.7+

  ```shell
     cf --version
  ```
</details>

## Understanding the Use Case

We want to build an application that helps users to sign up for an event (such as TechEd) and sessions (such as this tutorial) of the event.

When the user signs up for an event the following things should happen:
- The user should get registered for the event. 
- A learning goal should be automatically created for them in SuccessFactors. 
- Any subsequent sessions that a user signs up for should also be registered and added as sub-goals to the created goal.

Based on the use case we need components to handle signing up, registration, and goal creation.

We will use a synthetic remote OpenAPI service (https://ad266-registration.cfapps.eu10-004.hana.ondemand.com/api-docs) to register the user for an event/session.
For creating the goal in SuccessFactors, we will use the SAP SuccessFactors Goal Plan API (https://api.sap.com/api/PerformanceandGoalsPMGM/overview).

> Note: We are using a pre-existing project for this tutorial which is a Spring Boot CAP application.

Continue to - [Exercise 1 - Understand the Existing Project Setup](../ex1/README.md)

## Maintainer

This project is maintained by Manoj Gali, a Senior SAP CPI Consultant with over 5 years of experience in SAP integration technologies. Manoj specializes in SAP CPI, PI/PO, and hybrid integration landscapes, with deep technical expertise in Groovy Scripting, XSLT, and User-Defined Functions (UDFs). He focuses on designing and optimizing scalable integration solutions to ensure secure, high-performance data exchange across SAP and non-SAP systems.

Contact: manoj.gali695@gmail.com