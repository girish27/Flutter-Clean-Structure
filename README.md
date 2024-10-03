<<<<<<< HEAD
# flutter_project_structure

A new Flutter project where we try to dcribe the Flutter Clean Architecture

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
=======
# Flutter-Clean-Architecture
This repository serves as my personal documentation and learning journey in implementing Clean Architecture within Flutter applications. The objective is to build scalable, maintainable, and testable mobile apps by following the best practices of Clean Architecture principles.

## Intorduction
Clean Architecture is the blue print for a modular system which strictly follows the design principle called seperation of concerns more specifically this style of Architecture focuses on dividing software in to layers to simplify the development and maintenance of the system itself

### Clean Architecture is one of the most powerful solution to build clean apps with independent data layers that multiple teams can work on, scalable, readable, testable and can be easily maintained at any time

## The three main layes of the Architecture: 
Data Layer 

Domain Layer

Presentation or Feature Layer 

## Additional Supporting layers:

Resources

Shared Layers

# Data Layer
This is the outer most layer and is responsible for DATA RETRIEVAL this can be in the form of API CALLS TO A SERVER or LOCAL DATA BASE it also contains repository implementations this layer has 3 parts

Repositories:
It includes actual implementations of the reposiories in the domain layer, repositories are responsible to coordinate data from the different data sources.

Data Sources:
It consists of REMOTE and LOCAL data sources, remote data sources will perform HTTP request on the API while local data source will cache our persist data.

Models:
It represents the Json Structure and allows us to interect with our data sources


# Domain Layer
This is the inner part of the layer and has no dependency on other layer it should only be concedered with business logic of the application not with the implementaton details.
### NOTE: The Domain Layer would be written purely on Dart without any flutter Elements.

Entities:
The Entities must be "DATA TYPES" or "CLASSES" that are used in different parts of our app or in other word We define our version of clean that our entities are the objects that can be returned to us or we can send to an API.

Repository Interfaces:
Repositories are ABSTRACT CLASSES or CONTRACTS and defines the properties and methods that our project will need in a specific feature. 

Use cases:
Use case include application specific business rules, each event is the interaction of the user with the system and we can call this usecase like "sign up" "log in" and other interactions, Use Cases are nothing more than a bridge between layers, its a single call to business logic.

# Presentation Layer
This layer presents the App content and triggers events that modify the application state, this layer has 3 parts

Pages:
Which include Application Pages

State Management:
Files related to State Management that we use such as {BLOC,RIVERPOD,...}

Widgets:
which includes all the specific widgets that we use on the pages


  





>>>>>>> a08b47a84dee1f45535b21000a79be156ad22799
