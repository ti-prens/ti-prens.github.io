---
title: "How to build a drone from scratch"
date: 2017-08-02
type: "page"
tags: ["project","sample","Perso"]
categories: "Learning"
project_context: "Perso"
draft: false
genre: "project_perso"
type : "page"
---

# Zwazo

The "Zwazo" project is an initiative aimed at designing and building a drone from scratch. The goal is not to stop at mere experimentation or creating a basic prototype, but to rigorously follow the V-model, ensuring structured design and systematic validation at each stage of development. Special emphasis is placed on exercising skills that we do not want to lose or that we wish to acquire.

## Team and Organization

Our team consists of three technology and engineering enthusiasts: [Sofiane AOUCI](https://fr.linkedin.com/in/sofiane-aouci), [Daniel JACQUET](https://www.linkedin.com/in/jacquet-daniel-ba3653214/), and [Prince JACQUET](https://www.linkedin.com/in/prince-jacquet/).
We have set up the project structure on GitLab with continuous integration to ensure code quality and robustness.
We have also organized a home lab and acquired all the necessary components and tools for the development of the drone.

## Work Environment and Laboratory

To ensure smooth and methodical development, we have established a comprehensive work environment including:

- **Hardware:**
    - Soldering iron
    - Multimeter
    - Oscilloscope
    - Signal generator
    - Power supply
    - ...

- **Software:**
    - Software development: STM32 CubeMX, Cube IDE, CubeProgrammer, CMake, and ARM GCC
    - Electronic CAD: KiCad

![Home lab](/img/lab1_PXL_20240717_094138337.jpg)

## Progress and Key Stages

### Mechanical and Electrical Construction

After acquiring the mechanical components (propellers and drone structure), we successfully completed the mechanical and electrical stages of the drone:

- Assembly of the structure
- Wiring and power supply (battery and BMS)
- Installation of motors and ESCs

![Spinning propellers](/img/ezgif-2-a4b22c9f0d%20(Small).gif)

### First Testing Phase

#### Test Software Development

We used a microcontroller (Arduino dev board) and developed the minimum viable software to make the drone's structure take off.

#### First Test Flight

A first test flight was conducted to verify the lift and electromechanical functioning of the drone, marking a crucial milestone in the project's development.


![Re-wiring the drone](/img/rewiring_drone_PXL_20240717_094106382.jpg)

#### Testing the Development Infrastructure

Development of GPIO drivers is ongoing (approximately 25% complete) to test and validate our infrastructure. This includes organizing components, managing their dependencies, toolchains, and the overall development process.

## Project Structure and V-Model

### Management and Documentation

The project structure on GitLab, with continuous integration, allows for effective management and complete traceability of modifications. For project management, we are considering GitLab issues coupled with Jira tickets. Documentation is kept up to date for each component and self-references with internal wiki links to allow for documentation evolution alongside development.

### Project Architecture

Our broad approach is to follow the V-model, going through the following stages:

1. **Definition of Requirements**: Identification of functional and non-functional requirements.
2. **System Specification**: Definition of detailed technical specifications.
3. **Design**: Development of hardware and software architecture.
4. **Implementation**: Development and integration of hardware and software components, including the design of support tools and systems.
5. **Unit and Integration Testing**: Verification of each module in isolation and in interaction.
6. **Validation**: Validation of the complete system through testing in real conditions.

### Tools for Architecture? Not yet defined!

The project's architecture raises crucial questions regarding the tools and methods necessary to create, maintain, and evaluate the entire system.

Considering only the definition of requirements and the specification of systems (and of all subsystems), we are still hesitating between two choices: Capella or developing custom tools based on text files.

In one case, we would like to take advantage of all the benefits offered by Capella as a MBSE software, but this would contradict the "git-able" philosophy we wish to adopt, favoring a completely text-based approach.
In the other case, we have a lot of work to do and still have to enconter problematic that we are not used to.

## Involvement and Ambition

Here is a non-exhaustive list of our ambitions and objectives that we wish to achieve ourselves, in order of priority:

- **Electronic Design**: To carry out all the electronic design of the drone ourselves.
- **Embedded Software Development**: To create robust embedded software.
- **Automation**: To establish automation processes to facilitate development and testing.
- **Implementation of Continuous Integration**: To integrate CI/CD pipelines to ensure continuous and quality delivery.
- **Infrastructure Management**: To ensure effective and scalable infrastructure management.
- **Version Control**: To use version control systems for optimal traceability and collaboration.
- **Characterization and Modeling of the Drone**: To analyze and model the performance and characteristics of the drone.
- **Integration of Sensors and Data Fusion**: To integrate and optimize the use of sensors for effective data fusion.
- **Development of Architecture Tools in Markdown**: To create tools that allow documenting and managing the project architecture in Markdown files, with functionalities similar to Capella MBSE.

## Perspectives and Future Objectives

Our vision for the "Zwazo" project is to create a drone capable of performing complex tasks with advanced autonomy. The next steps include:

- **Edge AI**: Integrating artificial intelligence algorithms executable directly on the drone (edge computing) for optimal performance.

## Conclusion

The "Zwazo" project is an ambitious technological adventure committed to following a rigorous methodology, with the goals of:

- Creating a functional, reliable, and maintainable drone according to best practices.
- Collaborating with other enthusiasts to exercise and acquire interesting skills.

Our GitLab repository is private, but we publish articles about our progress irregularly ^^ at the following address: [https://prince.jacquet.live/](https://prince.jacquet.live/projects/).