# FRC Robot Codebase

This repository contains the official robot code for a FIRST Robotics Competition (FRC) team. It is organized to support rapid development, testing, and iteration during the build season and competition.

## Useful Links
- [2026 Java Code Guide](https://firstfrc.blob.core.windows.net/frc2026/KitBot/2026-kitbot-java-guide.pdf) This file helps explain how the code was set up. 
- [2026 Game manual](https://firstfrc.blob.core.windows.net/frc2026/Manual/2026GameManual.pdf)

## Purpose
- Control the robot during autonomous, teleoperated, and test modes
- Provide a clean structure for subsystems, commands, and robot-wide configuration
- Support simulation and debugging workflows used in FRC development

## Repository Structure
- `src/main/java` or `src/main/cpp` — Primary robot source code
- `src/main/resources` — Configuration files and assets
- `vendordeps/` — Third-party dependency definitions
- `build.gradle` / `gradlew` — Build and deployment tooling
- `.wpilib/` — WPILib project metadata

## Key Concepts
- **Robot lifecycle**: Code is organized around FRC robot modes (disabled, autonomous, teleop, test)
- **Subsystems**: Encapsulate robot mechanisms and shared state
- **Commands**: Define robot actions and behaviors
- **Container**: Central place for bindings, command setup, and configuration

## Build and Deployment
This project uses the standard WPILib build system.
- Build, deploy, and run tasks are handled through Gradle
- Simulation and unit testing are supported through WPILib tools

Refer to official WPILib documentation for environment setup and usage.

## Development Guidelines
- Keep subsystems cohesive and commands focused
- Avoid hardware access outside of subsystems
- Document non-obvious behavior and assumptions in code
- Test changes in simulation before deploying to a robot

## Version Control
- Commit frequently with clear messages
- Keep the main branch in a deployable state
- Use feature branches for experimental work

## License
This codebase is intended for educational and competition use. Licensing terms, if any, should be defined by the team.
