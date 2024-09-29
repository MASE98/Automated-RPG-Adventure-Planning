# Automated-RPG-Adventure-Planning
The fundamental purpose is the achievement of going from the initial level to the goal level, overcoming the challenges present in the different levels that make up a world within the game.

## Table of Contents

- [Project Structure](#project-structure)
- [Requirements](#requirements)
- [Instalación](#instalación)
- [Usage](#usage)
  - [Ejecución Local](#ejecución-local)
  - [Uso del Servicio REST](#uso-del-servicio-rest)
- [Example](#example)
- [Conclusion](#conclusion)
- [Developed](#developed)

## Project Structure
The Automated RPG Adventure Planning system is organized around the principles of automated planning. The project structure consists of two fundamental components: the domain and the problems:

### 1. Domain
- **domain.pddl**: Defines the general rules of the world in which the planning takes place, as well as the actions that the characters can perform. This includes the definition of:
- 
- **problems.pddl**: Analizador léxico que tokeniza el código ensamblador.

  ### 1. Domain

The **domain** describes the general rules and dynamics of the RPG world. It defines what actions characters can take and how those actions affect the state of the world. The main elements of the domain include:

- **actions**: These are operations that characters (or NPCs) can perform within the game, such as moving from one location to another, interacting with objects, or facing enemies. The actions are as follows:
- **move**: Un personaje se desplaza de una ubicación a otra.
  
- **Predicados**: Descripciones del estado del mundo que se utilizan para evaluar las condiciones de las acciones, como si un personaje se encuentra en una ubicación o si posee un objeto.
- **Objetos y personajes**: Entidades que existen en el entorno y que son relevantes para la planificación, como personajes, lugares o ítems.

### 2. Problemas

Los **problemas** son instancias específicas del dominio, en las cuales se definen:
- **Estado inicial**: La configuración inicial del mundo, es decir, la posición de los personajes, objetos y otros elementos del entorno antes de iniciar la planificación.
- **Objetivo**: El estado que se desea alcanzar. El planificador generará una secuencia de acciones que transformen el estado inicial en el estado objetivo.
- **Recursos y restricciones (opcional)**: En algunos casos, pueden añadirse limitaciones adicionales como tiempo, energía o inventario, para agregar más complejidad a la planificación.

### Ejemplo de Estructura

- **Dominio**: Definido en archivos que contienen la lógica y las reglas del mundo, como `domain.pddl` o `rpg_domain.py`.
- **Problemas**: Instancias específicas de la planificación almacenadas en archivos de configuración, como `problem_1.pddl` o `rpg_problem_1.py`, que establecen los estados inicial y objetivo para cada aventura o misión.

Esta estructura modular permite una fácil extensión del sistema, ya que se pueden agregar nuevas acciones al dominio o definir nuevos problemas para crear diferentes escenarios dentro del mundo RPG.
