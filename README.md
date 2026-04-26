# HOT-based SysML v2 View Generation Prototype

This repository contains a research prototype for generating customized SysML v2 views using a Higher-Order Transformation (HOT) approach.

## Overview

The prototype demonstrates how configurable view specifications can be used to automatically generate visualization templates (EGL) for SysML v2 models. These templates are then rendered using Picto as interactive HTML views.

The implementation focuses on enabling custom view generation without manually developing separate visualization templates.

## Important Note

This repository uses the Picto-SysMLv2 example project only as a **setup for integrating Picto, Epsilon, and SysML v2 into Eclipse**. 

No modifications have been made to the original example views. The research contribution of this repository lies in the `HOT_project` folder.

## Repository Structure

* `org.eclipse.epsilon.examples.picto.sysmlv2/` – Base project used to configure Picto and SysML v2 environment
* `HOT_project/` – Main research contribution, including:

  * Higher-Order Transformation (EOL)
  * EGX orchestration
  * JSON-based view specification
  * Generated EGL templates

## Prerequisites

* Eclipse IDE
* Epsilon 2.8 or later
* SysML v2 support for Eclipse

## Setup and Execution

Follow these steps to run the prototype:

1. Install Epsilon 2.8 or later on top of Eclipse.
2. Add SysML v2 to your Eclipse installation. (https://github.com/Systems-Modeling/SysML-v2-Release/tree/master/install/eclipse)
3. Clone this repository.
4. Import the `org.eclipse.epsilon.examples.picto.sysmlv2` project into your Eclipse workspace.
5. Right-click on the project and select:

   ```
   Run As → Eclipse Application
   ```
6. In the nested Eclipse workspace:

   * Import the `SysML_models` project.
7. Clone the SysML v2 repository. (https://github.com/Systems-Modeling/SysML-v2-Release)
8. Import the SysML library project into the nested workspace. (https://github.com/Systems-Modeling/SysML-v2-Release/tree/master/sysml.library)
9. Go to the preferences of the `SysML_models` project and add `sysml.library` to Project References.
10. Open:

    ```
    VehicleModel.sysml
    ```
11. Open Picto view:

    ```
    Window → Show View → Other → Picto
    ```
12. Select the generated view to visualize the model.

## Research Contribution

The main contribution of this repository is the use of a Higher-Order Transformation (HOT) to:

* Generate EGL-based visualization templates from a specification file
* Support configurable and reusable view generation
* Reduce the need for manual template development

## Acknowledgment

This work uses the Picto-SysMLv2 example project for environment setup:

https://github.com/kolovos/picto-sysmlv2

## License

Add an appropriate license if required.
# SysMLv2_Model_Visualization

