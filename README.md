# Doctorinna - medical risk factor analyzer
**Authors:** Lada Morozova, Denis Schegletov, Danis Alukaev, Maxim Pryanikov. \
**Group:** B19-DS-01, Innopolis University.

> This is the overview repository primarily used for documentation, implementation details see [Structure of project](#structure) section

Doctorinna is an application for determining the user's risk group for the widespread diseases by medical parameters. 
This application will allow people in the form of a survey without undergoing a medical examination to understand
whether it is necessary to be examined by a doctor and change their lifestyle.

### Motivation
A modern person prefers not to think about the fact that sooner or later his or her life will end. Our old age is so far away. So much so that it is easy for it to get lost in everyday studies, tedious work, questionable entertainment, quick snacks and hours of communication on social networks.

Doctorinna is our attempt to create a product that sobers the modern generation. This open-source product allows you to determine your risk group for the most common diseases by answering questions related to body parameters, habits and heredity. To do this, machine learning models will be trained on publicly available data from patients with diabetes, cardiovascular disease, stroke and lung cancer. The list of diseases will increase as the project develops. An important feature of the project will be a system of recommendations for improving your health.

Our goal is to distract you from the flow of digital garbage for at least a minute, and ask the question, _what are you doing to live to old age?_

### <a name="structure"> Structure of project </a>
It was decided to build a backend API implemented on the Django REST Framework. It will contain the business logic of the application.

In our opinion, the main flow of users might come through the web version of the application and the Telegram bot. 
Therefore, it was decided to implement them first within the framework of the Software System Analysis and Design course.

Accordingly, the code is distributed into 3 repositories: 
- [Backend](https://github.com/Doctorinna/backend)
- [Frontend](https://github.com/Doctorinna/frontend)
- [Telegram bot](https://github.com/Doctorinna/telegram-bot)

Each repository has a detailed description of how to launch correspondent side of the project locally.

### Glossary
- **Cardiovascular Disease** - disease is a general term for conditions affecting the heart or blood vessels.
- **Diabetes** - disease which is caused by a high level of blood glucose.
- **Stroke** - stroke occurs when the blood supply to part of your brain is interrupted or reduced, preventing brain tissue from getting oxygen and nutrients.
- **Lung cancer** - type of cancer that begins in the lungs.
- **REST** - architecture that are typically loosely based on HTTP methods to access resources via URL-encoded parameters and the use of JSON or XML to transmit data.
- **Microservice** - architecture that arranges an application as a collection of loosely-coupled services. Opposed to monolithic architecture.
- **CRUD** - Create, Read, Update, Delete - 4 basic operations of persistent storage.
- **Serializer/DTO** - data structure in backend that can be converted to JSON and back, and then send to frontend.
- **Entity/Model(Backend)** - data structure used in backend that is mapped to table in SQL database.
- **Repository** - Github repository of organization Doctorinna.
- **Component (Frontend)** - group of HTML elements, that can be reused multiple times and structuralized code.
- **Logger (Backend)** - log the information about all activities to retrieve bugs more easily.
- **Risk group** - medical risk group of user. There are 4 types of risk groups: no risk, low risk, medium risk, high risk.
- **Component (UML)** - modular part of the system that encapsulate the state and behavior of a number classifiers.
- **State manager (Frontend)** - object that controls state in all application and send this state to components.
- **Service (Backend)** - part of the Backend that contains business logic.
- **Controller/urls (Backend)** - part of the Backend that contains sending and receiving information using HTTP methods.
- **Local Storage** - persistent storage in browser that can store key-value pairs.
- **RUP** - Rational Unified Process.
- **SSR** - Server Side Rendering. Technique to render web page in server and deliver to client already rendered (but it can be rerendered later on client side).
- **Questionnaire** - set of questions that are answered by users, processed by system and results are displayed on user interface.
- **Bot** - Telegram bot.
- **User** - web Users of the web application or telegram bot.

