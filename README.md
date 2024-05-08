# HackathonProject
DISPLAY BOOKSHELVES
 
This is a Selenium based Automation Project on a website named UrbanLadder
 
Project Description 
1.	Search for "BookShelves" with price below Rs. 15000, Category any one (like Wall Shelves / Kid Bookshelves / Study Tables, etc) &  exclude out of stock. Sort by price "High to Low", fetch the top 3 items & print all details in console output.
2.	From Living, retrieve all items under any one of sub-menu items like  "Seating & Chairs" or "Living Storage". Also print the same in console output.
3.	Under "Gift cards", choose "Birthday/Anniversay"; Fill "Customize your gift card" with valid price & date and click "Next" button; Fill "To" & "From" details under "who is this lucky person" with any one email id invalid (example: without @ symbol) and click "Submit"; Capture & display the error message in console output. Then give valid email id & validate all the given details in the "Confirm Details" section
 
Tech Stack
- Java(Maven Project)
- Eclipse (4.30.0)
- ApachePOI (5.2.5)
- TestNG and (7.9.0)
- Cucumber (7.15.0) 
- ExtentReport (1.14.0)
- extentreports-cucumber7-adapter (1.14.0)
- JSON (1.1.1)
- Selenium Grid(selenium-server-4.18.1)
 
Folder Structure 
 Package 1: pageObjects
 	Class 1: BasePage.java
  	Class 2: BookshelvesHomePage.java
   	Class 3: GiftsCardHomePage.java
  	Class 4: LivingSubMenuPage.java
  	Class 5: SubmittedFormDetailsPage.java
   	Class 6: UrbanLadderHomePage.java
 
 Package 2: StepDefinitions
   	Class 1: Hooks.java
   	Class 2: StepDefinitionFile.java
 
  Package 3: testBase
    	Class 1: BaseClass.java
 
  Package 4: testScenarios
    	Class 1: TC_0001_SearchBookshelve.java
    	Class 2: TC_0002_BookshelvesDetails.java
    	Class 3: TC_0003_LivingMenuItems.java
    	Class 4: TC_0004_GiftCards.java
    	Class 5: TC_0005_ConfirmingFormDetails java
    	Class 6: TestRunnereFile.java (run this file to run using Cucumber)
 
   Package 5: utilities
     	Class 1: ExcelWrite.java
     	Class 2: ExtentReportManager.java
     	Class 3: JsonRead.java

Test Cases 
  Test Case 1 : Search the Bookshelve on UrbanLadder Website
  Test Case 2 : Fetch and store and print all Bookshelves in required conditions
  Test Case 3 : Fetch and store and print all submenu options under Living options
  Test Case 4 : Get Gift Card option and Fill Form for Gifts with valid and invalid details 
  Test Case 5 : verify the submitted data on confirmation page
