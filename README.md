# Software
GENERAL INFOO

PROJECT DETAILS
CEN 302 SOFTWARE ENGINEERING

Project Title: Recipe Manager
Team Name: EJ_GROUP

Team Leader:
Name: Julisa Loci
GitHub Username: julisaloci

Team Members:
Name: Ema Mihaj
GitHub Username: emihaj

Problem Statement:
In restaurant kitchens, managing a wide range of recipes can be chaotic and inefficient. Existing
systems often lack organization and user-friendliness, leading to difficulties in accessing and
utilizing recipes effectively. This can result in inconsistencies in culinary offerings, impacting the
overall dining experience for customers.

Solution Proposed:
To address these challenges, we propose developing a sophisticated Java-based Recipe Manager
program specifically tailored for restaurant use. This solution will provide chefs and kitchen staff
with a centralized platform to efficiently store, organize, and manage recipes. With intuitive
functionalities and a user-friendly interface, the Recipe Manager will streamline workflow,
enhance productivity, and ensure consistency in culinary offerings.

Project Scope:
Aim: Provide restaurants with a streamlined solution for recipe management to improve
operational efficiency and maintain consistency in culinary offerings.

Main Objectives:
● Implement user-friendly functionalities for browsing, editing, and exporting recipes.
● Develop an optimized search feature for quick access to specific recipes.
● Design a seamless user interface customized for restaurant environments.

Application Description:
The Recipe Manager is a robust Java application designed to simplify recipe management
specifically for restaurants. By providing a centralized platform for storing and organizing
culinary creations, it aims to alleviate the complexities associated with menu planning and
preparation. With intuitive browsing and search functionalities, the application enables chefs and
kitchen staff to swiftly access, modify, and experiment with recipes, thereby streamlining
workflow and making the culinary process more efficient.

Additionally, the Recipe Manager offers valuable insights into recipe popularity, ingredient
trends, and customer preferences through its advanced analytics capabilities. This enables
restaurants to make data-driven decisions, optimize menu offerings, and tailor their culinary
creations to meet the evolving tastes and preferences of their clientele. Ultimately, the Recipe
Manager serves as a strategic tool for restaurants to enhance operational efficiency, maintain
consistency in culinary offerings, and deliver exceptional dining experiences to their customer


Roles and Tasks Distribution

Team Leader:
● Oversees project development and ensures adherence to objectives and deadlines.
● Coordinates communication among team members.
● Assists with any technical challenges and provides support as needed.

Main Roles and Tasks:
Julisa Loci/Ema Mihaj:
● Both team members will work closely together throughout the development process,
sharing insights, providing feedback, and supporting each other to ensure the successful
completion of the project.
● GUI Design and Implementation. Backend Development and File Handling
● Responsible for implementing functionalities related to reading, writing, and managing
recipe data in files.
● Develops algorithms for efficient data retrieval and manipulation.
● Ensures proper error handling and data validation.
● Both team members will be responsible for testing their respective components
rigorously to identify and address any bugs or issues. Additionally, they will collaborate 
on integration testing to ensure the smooth functioning of the entire application.
● Documentation: Both team members will contribute to the documentation of their
respective components, including code documentation, user manuals, and any other
relevant documentation required for the project.


Phase II: User Requirements and Application Specifications
Submission Deadline: 18.03.2024, 23:59

Chosen Development Model:
● Agile Development Model
● Justification: Agile is selected due to its flexibility and adaptability, which allows
for iterative development and continuous feedback incorporation. This model suits
well for a project like Recipe Manager where requirements might evolve over
time, and stakeholders' feedback is crucial.


User Requirements:

a. Stakeholders:
● End-users: Chefs, kitchen staff, restaurant managers.
● Clients: Restaurant owners or managers.
● Developers: Team members involved in the development process.
● Other stakeholders: Potential investors, IT support personnel.

b. User Stories:
User Type: Chef (End-user)
● Requirement: As a chef, I want to easily search for recipes by keywords or
categories, so I can quickly access the recipe I need during cooking.
● Benefit: Improved efficiency in finding and utilizing recipes, leading to smoother
workflow in the kitchen.


Functional Requirements:

a. Brief Description:
● The system should allow users to search for recipes based on various criteria.
● It should provide options for creating, editing, and deleting recipes.
● Users should be able to categorize recipes into different types or cuisines.

b. Acceptance Criteria:
● User can search for recipes by name, ingredient, or category.
● User can create, edit, and delete recipes with appropriate permissions.
● Recipes can be tagged with categories and cuisines.


Non-Functional Requirements:

a. Brief Description:
● The system should be user-friendly, with intuitive navigation and controls.
● It should be responsive and performant, even with a large number of recipes.
● Security measures should ensure data privacy and integrity.

b. Acceptance Criteria:
● User interface elements are logically organized and labeled for easy
understanding.
● The system responds promptly to user interactions, with minimal latency.
● User data is encrypted in transit and at rest, and access control mechanisms are in
place.


Application Specifications:

a. Architecture:
● The system follows a layered architecture, with separate tiers for presentation,
application logic, and data storage.
● Communication between components follows RESTful principles for flexibility
and scalability.

b. Database Model:
● The database includes tables for storing recipes, users, categories, and other
relevant entities.
● Relationships between tables are established to maintain data integrity and support
querying.

c. Technologies Used:
● Language: Java
● Framework: JavaFX for GUI development
● Database: SQLite for local storage
● Other: Apache Maven for project management

d. User Interface Design:
● Wireframes and mockups showcase a clean and intuitive interface, allowing users
to easily navigate and interact with recipes.
● Consistent design elements and color schemes enhance user experience.

e. Security Measures:
● User authentication is implemented to control access to sensitive features.
● Data encryption is utilized to protect user information, both at rest and in transit.
● Regular security audits and updates are conducted to mitigate potential
vulnerabilities

Software Architecture:
The Recipe Manager application is designed with a layered architecture to ensure modularity and
separation of concerns. It consists of the following layers:

Presentation Layer: This layer includes the graphical user interface (GUI) developed using
JavaFX framework. It provides the interface for users to interact with the application and
includes components such as buttons, text fields, and menus.
Application Logic Layer: This layer contains the core logic of the application. It handles user
inputs from the GUI, processes data, and communicates with the data storage layer. This layer is
responsible for functionalities such as searching, editing, and deleting recipes.
Data Storage Layer: The data storage layer manages the persistent storage of recipe data. It
utilizes SQLite database for local storage, ensuring efficient data retrieval and manipulation. This
layer interacts with the application logic layer to provide access to recipe data.

Component Diagram:
GUI Component: Represents the graphical user interface developed using JavaFX.
Application Logic Component: Contains the core logic of the application, including
functionalities such as recipe management and search.
Data Storage Component: Handles the storage and retrieval of recipe data using SQLite
database.

Detailed Design:
Class Diagram:
The class diagram illustrates the structure of the Recipe Manager application, including the
classes and their relationship.

Recipe: Represents a generic recipe with attributes such as name and instructions.
Recipeable: Interface defining the method searchRecipe which is implemented by different
types of recipes.
DessertRecipe: Subclass of Recipe representing dessert recipes with an additional attribute type.
MainDishRecipe: Subclass of Recipe representing main dish recipes with an additional attribute
typeOfCuisine.
BeverageRecipe: Subclass of Recipe representing beverage recipes with an additional attribute
alcorNot.

Sequence Diagrams:
Sequence diagrams depict the interactions between different components of the system to
accomplish specific tasks. Below are simplified sequence diagrams for browsing recipes and
editing a recipe:

Browsing Recipes:
User → GUI: Clicks on Browse Recipes
GUI → Application Logic: Request to retrieve recipes
Application Logic → Data Storage: Retrieve recipe data
Data Storage → Application Logic: Recipe data
Application Logic → GUI: Display recipes

Editing Recipe:
User → GUI: Selects recipe to edit
GUI →Application Logic: Request to edit recipe
Application Logic → Data Storage: Retrieve recipe data for editing
Data Storage → Application Logic: Recipe data
Application Logic → GUI: Display recipe for editing
User → GUI: Makes changes to recipe
GUI → Application Logic: Submit edited recipe
Application Logic → Data Storage: Update recipe data

Database Design:
The database design for the Recipe Manager application involves tables to store recipe data
efficiently. Below is a simplified representation:
Recipes Table: Contains columns for recipe name, instructions, type (dessert, main dish,
beverage), type of cuisine (for main dish recipes), and alcohol content (for beverage recipes).

RecipeID Name Instructions Type TypeOfCuisine AlcorNot
1 Recipe 1 Instructions... Main Italian -
2 Recipe 2 Instructions... Dessert - -
3 Recipe 3 Instructions... Beverage - High

Modeling:
Use Case Diagram:
The use case diagram outlines the various actions that different types of users can perform within
the Recipe Manager application:
Chef: Can browse recipes, search for recipes, edit recipes, and export recipes.
Restaurant Manager: Can view recipe analytics and manage user accounts.
Developer: Involved in the development and maintenance of the application.
Activity Diagrams:
Activity diagrams illustrate the flow of activities within the Recipe Manager application. Below
is a simplified activity diagram for editing a recipe:
Activity 1: User selects recipe to edit.
Activity 2: Application retrieves recipe data for editing.
Activity 3: Application displays recipe for editing.
Activity 4: User makes changes to recipe.
Activity 5: Application submits edited recipe for update.

Activity Diagram: Editing a Recipe
User selects recipe to edit: The activity begins when the user selects a recipe from the list to
edit.
Application retrieves recipe data for editing: The application receives the request to edit a
recipe and retrieves the corresponding recipe data from the database.
Application displays recipe for editing: Once the recipe data is retrieved, the application
displays the recipe details on the GUI, allowing the user to make modifications.
User makes changes to recipe: The user interacts with the GUI to make changes to the recipe,
such as modifying ingredients or instructions.
Application submits edited recipe: After the user has finished editing the recipe, the
application receives the updated recipe data.
Data Storage updates recipe data: The application updates the recipe data in the database with
the changes made by the user.
Activity ends: The activity of editing the recipe concludes, and the user can continue using the
application for other tasks.

State Diagrams:
State diagrams represent the different states that an object can be in and how it transitions
between those states. In the context of the Recipe Manager application, state diagrams could be
used to represent the states of a recipe (e.g., editing, published, deleted) and how it transitions
between these states based on user actions.
State Diagram: Recipe States
State 1: Draft: The initial state of a recipe when it is created or being edited. In this state, the
recipe is not finalized, and changes can be made to its content.
State 2: Published: When the recipe is finalized and ready to be shared or viewed by users, it
transitions to the published state. In this state, the recipe is available for browsing and searching
within the application.
State 3: Archived: If the recipe is no longer relevant or needed, it can be archived. In this state,
the recipe is still stored in the database but is not actively displayed or accessible through the
user interface.
Transition 1: Edit: From the draft state, the recipe can transition back to the draft state if further
edits are required.

Transition 2: Publish: From the draft state, the recipe can transition to the published state once
it is finalized.
Transition 3: Unpublish: From the published state, the recipe can transition back to the draft
state if it needs to be updated or unpublished.
Transition 4: Archive: From any active state (draft or published), the recipe can be archived,
transitioning to the archived state.
Transition 5: Restore: From the archived state, the recipe can be restored, transitioning back to
either the draft or published state based on its previous state.
