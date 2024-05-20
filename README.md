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
        
        return name1.contains(keyword) || inst.contains(keyword);
    }
}

2.public class MainDishRecipe extends Recipe {
    private String typeOfCuisine; 

    @Override
    public boolean searchRecipe(String keyword) {
        String name = this.getName().toLowerCase();
        String instructions = this.getInstructions().toLowerCase();
        String cuisineType = this.getTypeOfCuisine().toLowerCase();
        
        return name.contains(keyword) || instructions.contains(keyword) || cuisineType.contains(keyword);
    }
}

3.public class BeverageRecipe extends Recipe {
    public String alcorNot; 

    @Override
    public boolean searchRecipe(String keyword) {
        String name = this.getName().toLowerCase();
        String instructions = this.getInstructions().toLowerCase();
        
        return name.contains(keyword) || instructions.contains(keyword);
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
@Override
public boolean searchRecipe(String keyword) {
    // Convert name and instructions to lowercase for case-insensitive search
    String name = this.getName().toLowerCase();
    String instructions = this.getInstructions().toLowerCase();
    
    // Check if the keyword exists in the name or instructions
    return name.contains(keyword) || instructions.contains(keyword);
}

In the MainDishRecipe class, polymorphism is demonstrated through the searchRecipe method,
which is tailored to the characteristics of main dish recipes. This method accounts for the type of
cuisine or origin of the dish, in addition to the name and instructions.
@Override
public boolean searchRecipe(String keyword) {
    // Convert name and instructions to lowercase for case-insensitive search
    String name = this.getName().toLowerCase();
    String instructions = this.getInstructions().toLowerCase();
    
    // Check if the keyword exists in the name, instructions, or type of cuisine
    if (name.contains(keyword) || instructions.contains(keyword) ||
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
File f = new File("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_megimenga\\src\\main\\java\\com\\mycompany\\recipebook_megimenga\\" + name);

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
File files = new File("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_megimenga\\src\\main\\java\\com\\mycompany\\recipebook_megimenga\\RecipesMD.txt");

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

// The program stores the data read from the files into List and ArrayLists, making use of the Collections framework.
List<String> information;
List<String> RecipesList;
ArrayList<String> titles;
// ...
RecipesList = Arrays.asList(fileRecipes.split("#"));

// The program makes use of the FileOutputStream which is an output stream for writing data or storing data to a file.
// Declare a FileOutputStream object
FileOutputStream fileOut;
try {
    // Initialize the FileOutputStream with the file path
    fileOut = new FileOutputStream("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_megimenga\\src\\main\\java\\com\\mycompany\\recipebook_megimenga\\RecipesMD.txt");
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


Introduction to the Project:
Our project is a Recipe Manager Application aimed at organizing and managing various recipes. The application will allow users to add, search, and categorize recipes based on their type, such as beverage, dessert, or main dish. It provides an intuitive interface for users to interact with their recipes effectively.

1) Java Program Codes:
BeverageRecipe.java:

package com.mycompany.recipebook_julisaloci;

public class BeverageRecipe extends Recipe {
    
    public String alcorNot;

    public String getAlcorNot() {
        return alcorNot;
    }

    public void setAlcorNot(String alcorNot) {
        this.alcorNot = alcorNot;
    }

    @Override
    public boolean searchRecipe(String keyword) {
        String name1 = this.getName().toLowerCase();
        String inst =this.getInstructions().toLowerCase();
        if(name1.contains(keyword) || inst.contains(keyword))
            return true;
        else 
            return false;
    }
}



DessertRecipe.java:

package com.mycompany.recipebook_julisaloci;

public class DessertRecipe extends Recipe {
    
    private String type;

    public String getType() {
        return type;
    }

    public void setType(String type) {
        this.type = type;
    }
    
    @Override
    public boolean searchRecipe(String keyword) {
        String name1 = this.getName().toLowerCase();
        String inst =this.getInstructions().toLowerCase();
        if(name1.contains(keyword) || inst.contains(keyword))
            return true;
        else 
            return false;
    }
}


MainDishRecipe.java:

package com.mycompany.recipebook_julisaloci;

public class MainDishRecipe extends Recipe {
    
    private String typeOfCuisine;

    public String getTypeOfCuisine() {
        return typeOfCuisine;
    }

    public void setTypeOfCuisine(String typeOfCuisine) {
        this.typeOfCuisine = typeOfCuisine;
    }
    
    @Override
    public boolean searchRecipe(String keyword) {
        String name1 = this.getName().toLowerCase();
        String inst =this.getInstructions().toLowerCase();
        if(name1.contains(keyword) || inst.contains(keyword) || this.getTypeOfCuisine().contains(keyword))
            return true;
        else 
            return false;
    }
}


Recipe.java:

package com.mycompany.recipebook_julisaloci;

public class Recipe implements Recipeable {
   
    private String name;  
    private String instructions;
   
    public Recipe(String name, String[] listOfIng, String instructions) {
        this.name = name;
        this.instructions = instructions;
    }

    public Recipe() {
        this.name = null;
        this.instructions = null;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getInstructions() {
        return instructions;
    }

    public void setInstructions(String instructions) {
        this.instructions = instructions;
    }

    @Override
    public boolean searchRecipe(String keyword) {
        String name1 = this.name.toLowerCase();
        String inst = this.instructions.toLowerCase();
        if(name1.contains(keyword) || inst.contains(keyword))
            return true;
        else 
            return false;
    }
}


Recipeable.java:
package com.mycompany.recipebook_julisaloci;

public interface Recipeable {
    boolean searchRecipe(String keyword);
}


GUI : 

/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/GUIForms/Application.java to edit this template
 */
package com.mycompany.recipebook_julisaloci;

import java.io.BufferedReader;
import java.io.BufferedWriter;
import java.io.File;
import java.io.FileNotFoundException;
import java.io.FileOutputStream;
import java.io.FileReader;
import java.io.FileWriter;
import java.io.IOException;
import java.nio.file.Files;
import java.nio.file.StandardOpenOption;
import java.util.ArrayList;
import java.util.Arrays;
import java.util.HashMap;
import java.util.List;
import java.util.Scanner;
import java.util.logging.Level;
import java.util.logging.Logger;
import javax.swing.JOptionPane;
import javax.swing.JTextArea;
import static java.nio.file.StandardOpenOption.*;
import javax.swing.ImageIcon;
import javax.swing.JButton;

/**
 *
 * @author Julisa Loci
 */
public class gui extends javax.swing.JFrame {

    List<String> information;
    List<String> RecipesList;
    ArrayList<String> titles;
    /**
     * Creates new form gui
     */
    // Need to read from the files to get the information on recipes
    // using # as divider between recipes
    public gui() {
        
        initComponents();
        this.setTitle("Julisa's Book of Recipes");
        
        
        titles = new ArrayList();
        
       
       this.jTextArea1.setWrapStyleWord(true);
       this.jTextArea1.setEditable(false);
       
       //icon magnifying glass for search button
       
       this.searchButton.setIcon(new ImageIcon("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_julisaloci\\src\\main\\java\\com\\mycompany\\recipebook_julisaloci\\icon.png"));
       
       //Reading Files with scanner - this file is for the titles.
       File fileTitles = new File("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_julisaloci\\src\\main\\java\\com\\mycompany\\recipebook_julisaloci\\TitlesMD.txt");
        Scanner fileTitle;
        try {
            fileTitle = new Scanner(fileTitles);
            
            while(fileTitle.hasNextLine()) {
               String Title = fileTitle.nextLine();
               titles.add(Title);
               
               
           }
        } catch (FileNotFoundException ex) {
            Logger.getLogger(gui.class.getName()).log(Level.SEVERE, null, ex);
        }
           
       // Reading the recipes files into a String variable
       File files = new File("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_julisaloci\\src\\main\\java\\com\\mycompany\\recipebook_julisaloci\\RecipesMD.txt");
       Scanner file;
       String fileRecipes = "";
        try {
            file = new Scanner(files);  
            while(file.hasNextLine()) {
                 fileRecipes += file.nextLine();
                 
       }
          
            
       
        } catch (FileNotFoundException ex) {
            Logger.getLogger(gui.class.getName()).log(Level.SEVERE, null, ex);
        }
        
        //replaces the symbol for new line with a new line
        fileRecipes = fileRecipes.replaceAll("\\\\n","\n");
      
        //creating a list containing recipes by using a symbol as a divider
       RecipesList = Arrays.asList(fileRecipes.split("#"));
       
       //reading extra information regarding the recipes
       // Reading the recipes files into a String variable
       File filesInfo = new File("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_julisaloci\\src\\main\\java\\com\\mycompany\\recipebook_julisaloci\\infosMD.txt");
       String fileInformation = "";
        try {
            file = new Scanner(filesInfo);  
            while(file.hasNextLine()) {
                 fileInformation += file.nextLine();
                 
       } 
       
        } catch (FileNotFoundException ex) {
            Logger.getLogger(gui.class.getName()).log(Level.SEVERE, null, ex);
        }
        information = Arrays.asList(fileInformation.split("\\\\n"));
       
       //Infos follow the format typeClass - name - type of dish/drink
     
       //putting the recipes along the titles in a hashmap
      
       for(int i=0; i < titles.size();i++) {
    
           String[] info = information.get(i).split("\\;");
           String category = info[0];
           String name = info[1];
           String cType = info[2];
           if(category.equals("MainDish")){
               MainDishRecipe rec = new MainDishRecipe();
               rec.setName(titles.get(i));
               rec.setInstructions(RecipesList.get(i));
               rec.setTypeOfCuisine(cType);
               recipes.put(titles.get(i), rec);
           }
           else if(category.equals("Dessert")){
               DessertRecipe rec = new DessertRecipe();
                rec.setName(titles.get(i));
                 rec.setInstructions(RecipesList.get(i));
                 rec.setType(cType);
               recipes.put(titles.get(i), rec);
           }
           else {
               //drink
               BeverageRecipe rec = new BeverageRecipe();
                rec.setName(titles.get(i));
                 rec.setInstructions(RecipesList.get(i));
                 if(cType.equals("Alcoholic")){
                 rec.setAlcorNot("Alcoholic");
                 } else if(cType.equals("Non-Alcoholic")) {
                     rec.setAlcorNot("Non-Alcoholic");
                 }
                
               recipes.put(titles.get(i), rec);
           }
           
          
       }
       
 
       
       
       
       
        
    } 


    /**
     * This method is called from within the constructor to initialize the form.
     * WARNING: Do NOT modify this code. The content of this method is always
     * regenerated by the Form Editor.
     */
    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">//GEN-BEGIN:initComponents
    private void initComponents() {

        jPanel1 = new javax.swing.JPanel();
        jPanel3 = new javax.swing.JPanel();
        jScrollPane1 = new javax.swing.JScrollPane();
        jTextArea1 = new javax.swing.JTextArea();
        jPanel2 = new javax.swing.JPanel();
        jLabel1 = new javax.swing.JLabel();
        jSeparator1 = new javax.swing.JSeparator();
        jComboBox1 = new javax.swing.JComboBox<>();
        jComboBox2 = new javax.swing.JComboBox<>();
        jComboBox3 = new javax.swing.JComboBox<>();
        jLabel2 = new javax.swing.JLabel();
        jButton1 = new javax.swing.JButton();
        jButton2 = new javax.swing.JButton();
        jButton3 = new javax.swing.JButton();
        jTextField1 = new javax.swing.JTextField();
        searchButton = new javax.swing.JButton();

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);

        jPanel1.setBackground(new java.awt.Color(245, 245, 245));

        jPanel3.setBackground(new java.awt.Color(250, 250, 250));

        jTextArea1.setColumns(20);
        jTextArea1.setLineWrap(true);
        jTextArea1.setRows(5);
        jScrollPane1.setViewportView(jTextArea1);

        javax.swing.GroupLayout jPanel3Layout = new javax.swing.GroupLayout(jPanel3);
        jPanel3.setLayout(jPanel3Layout);
        jPanel3Layout.setHorizontalGroup(
            jPanel3Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(jPanel3Layout.createSequentialGroup()
                .addContainerGap()
                .addComponent(jScrollPane1, javax.swing.GroupLayout.DEFAULT_SIZE, 313, Short.MAX_VALUE))
        );
        jPanel3Layout.setVerticalGroup(
            jPanel3Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(jPanel3Layout.createSequentialGroup()
                .addContainerGap()
                .addComponent(jScrollPane1)
                .addContainerGap())
        );

        jPanel2.setBackground(new java.awt.Color(248, 248, 240));

        jLabel1.setFont(new java.awt.Font("Arial", 1, 24)); // NOI18N
        jLabel1.setText("CATEGORIES");

        jComboBox1.setModel(new javax.swing.DefaultComboBoxModel<>(new String[] { "Main Dish", "Spaghetti Carbonara", "Baked potatoes", "Rice (Albanian Recipe)", "Burek with cheese" }));
        jComboBox1.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jComboBox1ActionPerformed(evt);
            }
        });

        jComboBox2.setModel(new javax.swing.DefaultComboBoxModel<>(new String[] { "Dessert", "Tiramisu", "Tres leches", "Brownies", " " }));
        jComboBox2.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jComboBox2ActionPerformed(evt);
            }
        });

        jComboBox3.setModel(new javax.swing.DefaultComboBoxModel<>(new String[] { "Beverages", "Strawberry  Banana Smoothie", "Christmas punch", "Hot cocoa", "" }));
        jComboBox3.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jComboBox3ActionPerformed(evt);
            }
        });

        jLabel2.setFont(new java.awt.Font("Arial", 1, 48)); // NOI18N
        jLabel2.setText("RECIPES");

        jButton1.setText("Export Recipe");
        jButton1.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton1ActionPerformed(evt);
            }
        });

        jButton2.setText("Delete");
        jButton2.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton2ActionPerformed(evt);
            }
        });

        jButton3.setText("Edit");
        jButton3.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton3ActionPerformed(evt);
            }
        });

        searchButton.setText("search");
        searchButton.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                searchButtonActionPerformed(evt);
            }
        });

        javax.swing.GroupLayout jPanel2Layout = new javax.swing.GroupLayout(jPanel2);
        jPanel2.setLayout(jPanel2Layout);
        jPanel2Layout.setHorizontalGroup(
            jPanel2Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, jPanel2Layout.createSequentialGroup()
                .addContainerGap(23, Short.MAX_VALUE)
                .addGroup(jPanel2Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING, false)
                    .addGroup(jPanel2Layout.createSequentialGroup()
                        .addComponent(jButton1)
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                        .addComponent(jButton3)
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                        .addComponent(jButton2))
                    .addComponent(jLabel2, javax.swing.GroupLayout.PREFERRED_SIZE, 283, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jComboBox3, javax.swing.GroupLayout.Alignment.TRAILING, 0, 294, Short.MAX_VALUE)
                    .addComponent(jComboBox2, javax.swing.GroupLayout.Alignment.TRAILING, 0, 294, Short.MAX_VALUE)
                    .addComponent(jComboBox1, javax.swing.GroupLayout.Alignment.TRAILING, 0, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                    .addComponent(jSeparator1, javax.swing.GroupLayout.PREFERRED_SIZE, 113, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jLabel1, javax.swing.GroupLayout.PREFERRED_SIZE, 283, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addGroup(jPanel2Layout.createSequentialGroup()
                        .addComponent(jTextField1, javax.swing.GroupLayout.PREFERRED_SIZE, 191, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                        .addComponent(searchButton, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)))
                .addGap(60, 60, 60))
        );
        jPanel2Layout.setVerticalGroup(
            jPanel2Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, jPanel2Layout.createSequentialGroup()
                .addContainerGap(javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                .addComponent(jLabel2, javax.swing.GroupLayout.PREFERRED_SIZE, 66, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                .addComponent(jSeparator1, javax.swing.GroupLayout.PREFERRED_SIZE, 15, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                .addComponent(jLabel1, javax.swing.GroupLayout.PREFERRED_SIZE, 32, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(14, 14, 14)
                .addComponent(jComboBox1, javax.swing.GroupLayout.PREFERRED_SIZE, 32, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(18, 18, 18)
                .addComponent(jComboBox2, javax.swing.GroupLayout.PREFERRED_SIZE, 32, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                .addComponent(jComboBox3, javax.swing.GroupLayout.PREFERRED_SIZE, 32, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(18, 18, 18)
                .addGroup(jPanel2Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(jButton1)
                    .addComponent(jButton3)
                    .addComponent(jButton2))
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                .addGroup(jPanel2Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(jTextField1, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(searchButton))
                .addContainerGap())
        );

        javax.swing.GroupLayout jPanel1Layout = new javax.swing.GroupLayout(jPanel1);
        jPanel1.setLayout(jPanel1Layout);
        jPanel1Layout.setHorizontalGroup(
            jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(jPanel1Layout.createSequentialGroup()
                .addComponent(jPanel2, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                .addComponent(jPanel3, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addContainerGap())
        );
        jPanel1Layout.setVerticalGroup(
            jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addComponent(jPanel3, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
            .addGroup(jPanel1Layout.createSequentialGroup()
                .addComponent(jPanel2, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                .addGap(29, 29, 29))
        );

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(0, 0, Short.MAX_VALUE))
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addComponent(jPanel1, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
        );

        pack();
    }// </editor-fold>//GEN-END:initComponents

    private void jComboBox1ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jComboBox1ActionPerformed
        // TODO add your handling code here:
        
        // Main dish selection, when selected, it should show the recipe on the right 
        String displayMD = this.jComboBox1.getSelectedItem().toString();
        this.jTextArea1.setText("");
        this.jTextArea1.setWrapStyleWord(true);
        if(this.jComboBox1.getSelectedIndex()!=0) {
          this.jTextArea1.append(this.recipes.get(displayMD).getInstructions());
          this.currentRecSel = this.jComboBox1.getSelectedItem().toString();
        }
        
        
    }//GEN-LAST:event_jComboBox1ActionPerformed

    private void jComboBox2ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jComboBox2ActionPerformed
        // TODO add your handling code here:
         String displayMD = this.jComboBox2.getSelectedItem().toString();
        this.jTextArea1.setText("");
        this.jTextArea1.setWrapStyleWord(true);
        if(this.jComboBox2.getSelectedIndex()!=0)  {
            this.jTextArea1.append(this.recipes.get(displayMD).getInstructions());{
             this.currentRecSel = this.jComboBox2.getSelectedItem().toString();
        }
        }
    }//GEN-LAST:event_jComboBox2ActionPerformed

    private void jComboBox3ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jComboBox3ActionPerformed
        // TODO add your handling code here:
         String displayMD = this.jComboBox3.getSelectedItem().toString();
        this.jTextArea1.setText("");
        this.jTextArea1.setWrapStyleWord(true);
        if(this.jComboBox3.getSelectedIndex()!=0){
            this.jTextArea1.append(this.recipes.get(displayMD).getInstructions());
             this.currentRecSel = this.jComboBox3.getSelectedItem().toString();
        }
    }//GEN-LAST:event_jComboBox3ActionPerformed

    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton1ActionPerformed
        // TODO add your handling code here:
       //When this button is clicked, export the showing recipe on the JTextArea
       String recipe = this.jTextArea1.getText();
      
       //Keeping track of the exported number of recipes
       String name = "recipe"+exported+".txt";
       File f = new File("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_julisaloci\\src\\main\\java\\com\\mycompany\\recipebook_julisaloci\\"+name);
        if(!f.exists()){
           try {
               f.createNewFile();
               exported++;
             
               FileOutputStream outputFile = new FileOutputStream(f);
               byte[] fb = recipe.getBytes();
               outputFile.write(fb);
               JOptionPane.showMessageDialog(this, "Done");
               
              
           } catch (IOException ex) {
               Logger.getLogger(gui.class.getName()).log(Level.SEVERE, null, ex);
           }
}
    }//GEN-LAST:event_jButton1ActionPerformed

    private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton2ActionPerformed
        // TODO add your handling code here:
        //Delete 
        if(this.jComboBox1.getSelectedItem()!=this.jComboBox1.getItemAt(0)) {
        this.jComboBox1.removeItem(this.jComboBox1.getSelectedItem());}
        else if(this.jComboBox2.getSelectedItem()!=this.jComboBox2.getItemAt(0)) {
         this.jComboBox2.removeItem(this.jComboBox2.getSelectedItem());
        }
        else if(this.jComboBox3.getSelectedItem()!=this.jComboBox3.getItemAt(0)) {
            this.jComboBox3.removeItem(this.jComboBox3.getSelectedItem());
        }
        
    }//GEN-LAST:event_jButton2ActionPerformed

    private void jButton3ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton3ActionPerformed
        // TODO add your handling code here:
        //This button saves the edit made to the selection, the change in recipe
        //if the button's current text says "Done", means we are in Edit Mode
        
        if(this.jButton3.getText().equals("Done")) {
        
        String recUpdated = this.jTextArea1.getText();
        
             //find index 
          
    int index = 0;
     for(int i = 0; i < this.titles.size();i++) {
       if(titles.get(i).equals(this.currentRecSel)){
           index = i;
           break;
       }
      
     } 
      
        this.RecipesList.set(index, recUpdated);
        this.recipes.get(this.currentRecSel).setInstructions(recUpdated);
        
        this.jButton3.setText("Edit");
        this.jTextArea1.setEditable(false);
      
//write to file  -  UPDATE the file which stores the recipes with the edited Instructions
      File filesInfo = new File("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_julisaloci\\src\\main\\java\\com\\mycompany\\recipebook_julisaloci\\RecipesMD.txt");
       String fileInformation = "";
       int i = 0;
       //add n to each line and # as divider between recipes
       for(String a: RecipesList) {
           for( String b: a.split("\n")){
             fileInformation = fileInformation + b + "\\" + "n"+"\n";
             
           }
             fileInformation = fileInformation + "\n";
             fileInformation= fileInformation + "#";
             fileInformation= fileInformation + "\n";
           
       }
     //Update file w string
        FileOutputStream fileOut;
        try {
            fileOut = new FileOutputStream("C:\\Users\\hp\\Documents\\NetBeansProjects\\recipebook_julisaloci\\src\\main\\java\\com\\mycompany\\recipebook_julisaloci\\RecipesMD.txt");
            fileOut.write(fileInformation.getBytes());
            
            fileOut.close();
        } catch (Exception ex) {
            Logger.getLogger(gui.class.getName()).log(Level.SEVERE, null, ex);
        }
        this.revalidate();
         }  
        
    else if(this.jButton3.getText().equals("Edit")){
         this.jButton3.setText("Done");
          //make it non editable
         this.jTextArea1.setEditable(true);
         //change the text
         this.revalidate();
     }
        
  
   
    }//GEN-LAST:event_jButton3ActionPerformed

    private void searchButtonActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_searchButtonActionPerformed
        // Search for a recipe containing the words in the search barin the title
        String searchIt = this.jTextField1.getText().toLowerCase();
        // Search the titles
       this.jTextArea1.setText("");
       this.jTextArea1.setEditable(false);
       if(this.jTextField1.getText()!="") {
       for(String r:this.recipes.keySet()){
         
           if(this.recipes.get(r).searchRecipe(searchIt)==true){
               this.jTextArea1.append(this.recipes.get(r).getInstructions());
                this.repaint();
                break;
           }
       }
       }
    

       
       /* different way of searching 
     for(int i = 0; i < this.titles.size();i++) {
         String title = titles.get(i);
         title = title.toLowerCase();
         String rec1 = this.recipes.get(titles.get(i)).getInstructions();
         rec1 = rec1.toLowerCase();
       if(title.contains(searchIt)){
           JOptionPane.showMessageDialog(rootPane, "Done!");
           this.jTextArea1.append(this.recipes.get(titles.get(i)).getInstructions());
           this.repaint();
           break;
       }
       else if(rec1.contains(searchIt)) {
           this.jTextArea1.append(this.recipes.get(titles.get(i)).getInstructions());
           this.repaint();
           break;
       }
    */
      
     
     
                
           
    }//GEN-LAST:event_searchButtonActionPerformed

    /**
     * @param args the command line arguments
     */
    public static void main(String args[]) {
        /* Set the Nimbus look and feel */
        //<editor-fold defaultstate="collapsed" desc=" Look and feel setting code (optional) ">
        /* If Nimbus (introduced in Java SE 6) is not available, stay with the default look and feel.
         * For details see http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html 
         */
        try {
            for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
                if ("Nimbus".equals(info.getName())) {
                    javax.swing.UIManager.setLookAndFeel(info.getClassName());
                    break;
                }
            }
        } catch (ClassNotFoundException ex) {
            java.util.logging.Logger.getLogger(gui.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(gui.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(gui.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(gui.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        //</editor-fold>

        /* Create and display the form */
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new gui().setVisible(true);
            }
        });
    }

    // Variables declaration - do not modify//GEN-BEGIN:variables
    private javax.swing.JButton jButton1;
    private javax.swing.JButton jButton2;
    private javax.swing.JButton jButton3;
    private javax.swing.JComboBox<String> jComboBox1;
    private javax.swing.JComboBox<String> jComboBox2;
    private javax.swing.JComboBox<String> jComboBox3;
    private javax.swing.JLabel jLabel1;
    private javax.swing.JLabel jLabel2;
    private javax.swing.JPanel jPanel1;
    private javax.swing.JPanel jPanel2;
    private javax.swing.JPanel jPanel3;
    private javax.swing.JScrollPane jScrollPane1;
    private javax.swing.JSeparator jSeparator1;
    private javax.swing.JTextArea jTextArea1;
    private javax.swing.JTextField jTextField1;
    private javax.swing.JButton searchButton;
    // End of variables declaration//GEN-END:variables
     HashMap<String, Recipe> recipes = new HashMap<String, Recipe>();
     int exported = 0; //keeps count of the export no to generate multiple files with diff names.
     String currentRecSel = null;
     Recipe searchedRec;
   
    
}


This GUI class is responsible for providing a graphical interface for the Recipe Manager Application. Here's how it works:

Initialization: Upon initialization, the GUI reads recipe information from files, including titles, recipes, and additional information.

Display: The main window displays categories of recipes in combo boxes (Main Dish, Dessert, Beverages). When a category is selected, it displays the corresponding recipe in the text area.

Export: Users can export the displayed recipe by clicking the "Export Recipe" button. This action creates a new text file with the recipe content.

Delete: Users can delete a recipe by selecting it from the combo boxes and clicking the "Delete" button.

Edit: Users can edit a recipe by selecting it from the combo boxes, making changes in the text area, and clicking the "Edit" button. When in "Edit" mode, the button changes to "Done," indicating that changes are being saved.

Search: Users can search for recipes by typing keywords in the search bar and clicking the "Search" button. The GUI then displays the first recipe that matches the search criteria.

This GUI class integrates with the Recipe classes (BeverageRecipe, DessertRecipe, MainDishRecipe) and utilizes them to manage recipe data effectively.

To use this GUI class effectively, integrate it with the Recipe classes and ensure that the file paths for reading and writing recipe information are correctly set.

Overall, this GUI class provides a user-friendly interface for managing recipes efficiently.

