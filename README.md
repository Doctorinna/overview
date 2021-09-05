# Doctorinna - medical risk factor analyzer
**Authors:** Lada Morozova, Denis Schegletov, Danis Alukaev, Maxim Pryanikov. \
**Group:** B19-DS-01, Innopolis University.

Doctorinna is an application for determining the user's risk group for the widespread diseases by medical parameters. 
This application will allow people in the form of a survey without undergoing a medical examination to understand
whether it is necessary to be examined by a doctor and change their lifestyle.

### Motivation
A modern person prefers not to think about the fact that sooner or later his or her life will end. Our old age is so far away. So much so that it is easy for it to get lost in everyday studies, tedious work, questionable entertainment, quick snacks and hours of communication on social networks.

Doctorinna is our attempt to create a product that sobers the modern generation. This open-source product allows you to determine your risk group for the most common diseases by answering questions related to body parameters, habits and heredity. To do this, machine learning models will be trained on publicly available data from patients with diabetes, cardiovascular disease, stroke and lung cancer. The list of diseases will increase as the project develops. An important feature of the project will be a system of recommendations for improving your health.

Our goal is to distract you from the flow of digital garbage for at least a minute, and ask the question, _what are you doing to live to old age?_

### Structure of project
It was decided to build a backend API implemented on the Django REST Framework. It will contain the business logic of the application.

In our opinion, the main flow of users might come through the web version of the application and the Telegram bot. 
Therefore, it was decided to implement them first within the framework of the Software System Analysis and Design course.

Accordingly, the code is distributed into 3 repositories: 
- [Backend](https://github.com/Doctorinna/backend)
- [Frontend](https://github.com/Doctorinna/frontend)
- [Telegram bot](https://github.com/Doctorinna/telegram-bot)

Each repository has a detailed description of how to launch correspondent side of the project locally.

