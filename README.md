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



Software Testing
1. Introduction to Testing:
The Recipe Manager is a Java program designed to store and manage a collection of recipes. The
goal of the program is to provide a user-friendly interface that allows users to easily access and
manage their favorite recipes. The target audience is anyone who enjoys cooking and wants an
easy way to store and organize their recipes. This program helps the audience by providing a
centralized location to store all their recipes, making it easy to explore, store, edit, and export
them as needed.Software testing is a critical aspect of the development process, ensuring the
reliability and correctness of the Recipe Manager. By systematically evaluating the software
through testing, we can detect and rectify any defects or bugs, thereby enhancing the overall user
experience and ensuring the success of the program.
2. Purpose of Testing:
Identifying defects early:
Early testing allows us to uncover and address bugs in the initial stages of development,
minimizing the risk of costly fixes later on. By conducting thorough testing throughout the
development lifecycle, we can identify and resolve issues promptly, ensuring the stability and
reliability of the Recipe Manager.
Verification of functionality:
Testing serves to verify that all software components, including recipe storage, browsing, editing,
and exporting functionalities, perform as intended. By rigorously testing each component against
specified requirements and user expectations, we can ensure that the Recipe Manager meets its
intended purpose and delivers a seamless user experience.
Ensuring reliability:
Thorough testing enhances the reliability of the Recipe Manager by identifying and eliminating
potential sources of errors or failures. By subjecting the software to various test scenarios and
conditions, we can validate its robustness and resilience, reducing the likelihood of unexpected
issues during usage.
Improving software quality:
Testing contributes to improving the overall quality and stability of the Recipe Manager by
identifying and addressing defects. By systematically identifying areas for improvement and
implementing corrective measures, we can deliver a high-quality product that meets the needs
and expectations of its users.
3. Focus on Testing a Single Component:
In this phase, our testing efforts will be concentrated on a critical component of the Recipe
Manager: the Recipe class. The Recipe class encapsulates the attributes and functionalities of
individual recipes, making it essential to ensure its correctness and reliability. Testing this
component involves validating various functionalities, such as adding ingredients, deleting
ingredients, and updating instructions, to ensure that they behave as expected under different
scenarios.
4. Preparing Test Cases:
To prepare comprehensive test cases for the Recipe class, we will consider a wide range of
scenarios, including normal inputs, edge cases, and invalid inputs. Each test case will target
specific functionalities of the Recipe class, such as adding ingredients, deleting ingredients, and
updating instructions. Additionally, we will incorporate concepts such as inheritance and
polymorphism into our test cases to ensure thorough coverage of the Recipe class's behavior.
5. Choosing Testing Frameworks:
Given that our project is implemented in Java, we will utilize JUnit as the testing framework for
unit testing. JUnit offers robust support for writing and executing unit tests in Java, making it
ideal for our requirements. We will integrate JUnit into our development environment and
configure test suites to facilitate efficient testing of the Recipe class.
6. Writing Test Code:
We will develop test code for the Recipe class, focusing on creating test methods to exercise
different functionalities. Test methods will cover scenarios such as adding ingredients, deleting
ingredients, and updating instructions. Assertions will be utilized to validate expected outcomes
and ensure the correctness of the Recipe class implementation. Additionally, we will leverage
JUnit's annotations and assertions to streamline the testing process and improve code readability.
import static org.junit.Assert.*;
import org.junit.Test;
public class RecipeTest {
@Test
public void testAddIngredient() {
// Create a new Recipe instance
Recipe recipe = new Recipe("Chocolate Cake", "Delicious chocolate cake recipe");
// Add an ingredient to the recipe
recipe.addIngredient("Flour", "2 cups");
// Check if the ingredient was added successfully
assertTrue(recipe.getIngredients().containsKey("Flour"));
assertEquals("2 cups", recipe.getIngredients().get("Flour"));
}
@Test
public void testDeleteIngredient() {
// Create a new Recipe instance
Recipe recipe = new Recipe("Chocolate Cake", "Delicious chocolate cake recipe");
// Add an ingredient to the recipe
recipe.addIngredient("Sugar", "1 cup");
// Delete the ingredient from the recipe
recipe.deleteIngredient("Sugar");
// Check if the ingredient was deleted successfully
assertFalse(recipe.getIngredients().containsKey("Sugar"));
}
@Test
public void testUpdateInstructions() {
// Create a new Recipe instance
Recipe recipe = new Recipe("Chocolate Cake", "Delicious chocolate cake recipe");
// Update the instructions of the recipe
recipe.updateInstructions("Mix all ingredients together and bake at 350°F for 30 minutes.");
// Check if the instructions were updated successfully
assertEquals("Mix all ingredients together and bake at 350°F for 30 minutes.",
recipe.getInstructions());
}
}
7. Running Tests:
To execute the tests, we will run the test suite containing the test classes using JUnit. We will
analyze the test results to ensure that all tests pass successfully. In cases where tests fail or
encounter errors, we will investigate the issues and make necessary corrections to the Recipe
class implementation to address any identified defects. Continuous integration and automated
testing will be leveraged to streamline the testing process and ensure the reliability and stability
of the Recipe Manager.
8. Test Coverage:
Achieving high test coverage is essential to ensure thorough testing of the Recipe Manager
software. We aim to cover a significant portion of the Recipe class's codebase with our tests,
encompassing both functional and edge cases. By achieving high test coverage, we can enhance
confidence in the reliability and correctness of the Recipe Manager, delivering a robust and
stable product to our users. We will utilize code coverage tools to measure test coverage and
identify areas for improvement, ensuring that our testing efforts are comprehensive and effective.
9.Main functionalities of the Recipe Manager program are:
● Read a recipe
● Browse through recipes
● Edit a recipe
● Delete a recipe
● Export a recipe to a .txt file
● Search for a recipe
10.Project Development/Method Explanation
The Recipe Manager program uses various Java concepts to implement its functionality. The
program uses classes to represent different types of recipes, with inheritance and polymorphism
used to allow for the creation of specialized subclasses of the Recipe class. The program also
uses a GUI to make it easy for users to interact with the program and manage their recipes. In
addition, the program uses files to store and read recipe data, and collections to manage the
recipes.
11.The development of this program involves the utilization of specific
concepts, including:
➢ Classes:
Several classes are employed, each serving a distinct purpose within the program:
● Recipe.java
● DessertRecipe
● MainDishRecipe
● BeverageRecipe
● Recipeable
● Gui
➢ Inheritance:
Inheritance is implemented to establish relationships between classes, facilitating code reuse and
organization.
Notably, the classes DessertRecipe, MainDishRecipe, and BeverageRecipe inherit attributes and
behaviors from the parent class Recipe through the use of the extends keyword.
1.public class DessertRecipe extends Recipe {
private String type; // Only one variable declaration in this class
// Method to search for a recipe, utilizing fields from the superclass
public boolean searchRecipe(String keyword) {
String name1 = this.getName().toLowerCase();
String inst = this.getInstructions().toLowerCase();
if (name1.contains(keyword) || inst.contains(keyword)) {
return true;
} else {
return false;
}
}
}
2.public class MainDishRecipe extends Recipe {
private String typeOfCuisine; // Single variable declaration for this class
// Method overriding to search for a recipe, incorporating fields from the superclass
@Override
public boolean searchRecipe(String keyword) {
String name1 = this.getName().toLowerCase();
String inst = this.getInstructions().toLowerCase();
if (name1.contains(keyword) || inst.contains(keyword) ||
this.getTypeOfCuisine().contains(keyword)) {
return true;
} else {
return false;
}
}
}
3.public class BeverageRecipe extends Recipe {
public String alcorNot; // Single variable declaration for this class
// Method overriding to search for a recipe, utilizing fields from the superclass
@Override
public boolean searchRecipe(String keyword) {
String name1 = this.getName().toLowerCase();
String inst = this.getInstructions().toLowerCase();
if (name1.contains(keyword) || inst.contains(keyword)) {
return true;
} else {
return false;
}
}
}
➢ Polymorphism
Polymorphism is evident in this program through the implementation of methods in different
ways, tailored to the specific characteristics of each recipe type. For instance, when searching for
a beverage recipe, the search method considers the type of the drink, while for a MainDish
recipe, it accounts for the origin or type of the dish.
In the BeverageRecipe class, the searchRecipe method takes into account the attribute
"AlcorNot". However, in other classes such as MainDishRecipe, it considers the attribute
"typeOfCuisine", and in the DessertRecipe class, it utilizes the attribute "type".
// Example of polymorphism in the BeverageRecipe class
@Override
public boolean searchRecipe(String keyword) {
// Convert name and instructions to lowercase for case-insensitive search
String name1 = this.getName().toLowerCase();
String inst = this.getInstructions().toLowerCase();
// Check if the keyword exists in the name or instructions
if (name1.contains(keyword) || inst.contains(keyword)) {
return true;
} else {
return false;
}
}
In the MainDishRecipe class, polymorphism is demonstrated through the searchRecipe method,
which is tailored to the characteristics of main dish recipes. This method accounts for the type of
cuisine or origin of the dish, in addition to the name and instructions.
@Override
public boolean searchRecipe(String keyword) {
// Convert name and instructions to lowercase for case-insensitive search
String name1 = this.getName().toLowerCase();
String inst = this.getInstructions().toLowerCase();
// Check if the keyword exists in the name, instructions, or type of cuisine
if (name1.contains(keyword) || inst.contains(keyword) ||
this.getTypeOfCuisine().contains(keyword)) {
return true;
} else {
return false;
}
}
Interfaces
The program implements interfaces by having an Interface class called Recipeable which
requires the classes to implement, the searchRecipe method in different ways, a method to search
if a String is contained in any of their attributes to help the user search for the recipe in a better
way.
GUI
One of the most important features that ties everything together is the Graphical User Interface.
The GUI is developed using NetBeans and some features are coded/written independently from
the Netbeans GUI builder. The GUI is designed in a form that allows the user to quickly browse
through the elements of drop down lists and preview more information regarding each selection.
Exceptions
When dealing with file readings, editing and file exporting, the use of exceptions through a
try-catch block helps the program behave more and break less.
Example when exporting to a file
// When the export button is clicked, export the recipe displayed in the JTextArea
String recipe = this.jTextArea1.getText();
// Keeping track of the exported number of recipes
String name = "recipe" + exported + ".txt";
File f = new
File("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_megimenga\\src\\main\\java\\co
m\\mycompany\\recipebook_megimenga\\" + name);
// Check if the file already exists
if (!f.exists()) {
try {
// Create a new file
f.createNewFile();
exported++;
// Write the recipe content to the file
FileOutputStream outputFile = new FileOutputStream(f);
byte[] fb = recipe.getBytes();
outputFile.write(fb);
outputFile.close();
// Display a message to indicate successful export
JOptionPane.showMessageDialog(this, "Done");
} catch (IOException ex) {
// Handle IOException
Logger.getLogger(gui.class.getName()).log(Level.SEVERE, null, ex);
}
}
Files
This program does not use a database, therefore we use files as a way to store our data. The
program reads from files the recipes, titles and information. It exports to files the recipe that the
user wants to export and allows the user to edit a recipe through the program by performing this
edit on the original file.
Example for reading from a file
// Define the file path
File files = new
File("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_megimenga\\src\\main\\java\\co
m\\mycompany\\recipebook_megimenga\\RecipesMD.txt");
// Initialize a Scanner to read from the file
Scanner file;
String fileRecipes = "";
try {
// Open the file for reading
file = new Scanner(files);
// Read each line of the file
while (file.hasNextLine()) {
// Append each line to the fileRecipes string
fileRecipes += file.nextLine();
}
} catch (FileNotFoundException ex) {
// Handle file not found exception
Logger.getLogger(gui.class.getName()).log(Level.SEVERE, null, ex);
}
// Replace the symbol for a new line with an actual new line character
fileRecipes = fileRecipes.replaceAll("\\\\n", "\n");
// Create a list containing recipes by splitting the fileRecipes string using a symbol as a divider
RecipesList = Arrays.asList(fileRecipes.split("#"));
Collections
The program stores the data read from the files into List and ArrayLists, making use of the
Collections framework.
List<String> information;
List<String> RecipesList;
ArrayList<String> titles;
…
RecipesList = Arrays.asList(fileRecipes.split("#"));
Streams
The program makes use of the FileOutputStream which is an output stream for writing data or
storing data to a file.
// Declare a FileOutputStream object
FileOutputStream fileOut;
try {
// Initialize the FileOutputStream with the file path
fileOut = new
FileOutputStream("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_megimenga\\src\\
main\\java\\com\\mycompany\\recipebook_megimenga\\RecipesMD.txt");
// Write the data (fileInformation) to the output stream
fileOut.write(fileInformation.getBytes());
// Close the output stream
fileOut.close();
} catch (Exception ex) {
// Handle any exceptions that occur during the file operation
Logger.getLogger(gui.class.getName()).log(Level.SEVERE, null, ex);
}
// Revalidate the GUI (assuming this is a Swing or similar GUI component)
this.revalidate();
