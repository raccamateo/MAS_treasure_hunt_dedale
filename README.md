# MAS_treasure_hunt_dedale

## Introduction

This project is a sophisticated Java-based multi-agent system using the Dedale framework, designed for a treasure hunt game. It involves complex agent interactions and coordination within an initially unknown environment that the agents must explore.

## Installation

Prerequisites include Java JDK 8+ and Maven. Follow these steps:

1. Clone the repository: [https://github.com/raccamateo/MAS_treasure_hunt_dedale]
2. Open the project in IntelliJ as a Maven project (navigate to the inner `dedale-etu` folder).
3. Trust the project if prompted, and configure Maven as detailed in the provided guide.

Dependencies:

The project requires the following dependencies to be installed:
* JavaFX (version 18) modules including:
    * javafx
    * javafx-web
    * javafx-swing
    * javafx-media
    * javafx-graphics
    * javafx-fxml
    * javafx-controls
    * javafx-base
* JADE (Java Agent DEvelopment Framework) for multi-agent systems:
    * jade (version master-SNAPSHOT)
* GraphStream, a library for graph modeling and visualization:
    * gs-core (version 2.0)
    * gs-algo (version 2.0)
    * gs-ui-javafx (version 2.0)
    * gs-ui-swing (version 2.0)
* Bouncy Castle for cryptography:
    * bcmail-jdk14 (version 139)
* PlantUML for generating UML diagrams from a simple text description:
    * plantuml (version 8036)
* JUnit for unit testing:
    * junit (version 4.12)
* Jackson for JSON processing:
    * jackson-databind (version 2.12.3)
    * jackson-core (version 2.12.3)
* Dedale, the core project and Delta for specialized functionalities:
    * dedale (version -SNAPSHOT)
    * mas from com.gitlab.deltas (version -SNAPSHOT)
    * tools from com.gitlab.herpsonc (version -SNAPSHOT)
These dependencies are managed by Maven and should be automatically resolved and downloaded when building the project.

## Execution

Run the simulation using Maven:

    mvn install exec:java

The JADE and Dedale GUIs will open, and agents will be created and displayed.

## Configuration

Configure Dedale to use specific maps and elements:

1. Set `ConfigurationFile` to use the map and elements files.
2. Modify the `Principal` class to create agents with specified configurations.

## Agent Implementation and Dedale Usage

Agents utilize Dedale's functionalities for exploration, communication, and interaction:

- Agents communicate using ACL messages with protocols like "UselessProtocol".
- The `MapRepresentation` class manages the topology for navigation and strategy.
- Agents like `ExploreCoopAgent` and `CollectorAgent` are configured with specific attributes for tasks such as cooperative exploration and resource collection.

## Exercise Guide

The included guide details a comprehensive exercise for configuring and extending the simulation. It includes:

- Map and elements configuration.
- JSON configuration files for agents.
- Agent spawning and behavior customization.

## Contribution

Contribute to this Dedale-based simulation by:

1. Forking the repository.
2. Creating a feature branch.
3. Implementing new features or improvements.
4. Submitting a pull request with a complete description of changes.

## Acknowledgements

This project is developed on the Dedale framework, an educational tool for multi-agent systems provided by URV. The simulation is intended for educational and research purposes in the field of artificial intelligence, precisely on Multi Agent Systems.

Thank you for your interest and contributions!
