# NileshKaingade_SSEAIRTRICITY
E2E Automation Using SpecFlow C# Selenium Testing Framework - WebDriver

#How to Run :-

          Search solution explorer Left click - Clean solution Then - Build

          In Menu Test --> Windows --> Test explorer
          Run all

#Troubleshoot tips :- Make sure you have all updated packages

#Keywords : page object model c# selenium specflow c# page object model example specflow page object model pagefactory is obsolete c# selenium pagefactory c# selenium pagefactory c# deprecated page object model with pagefactory in selenium page object model for selenium scripting

#Framework Folder Structure -

Below is the main component of Framework -

A. Component Helper    
B. Configuration    
C. Features  
D. Page Object    
E. Settings  
F. Step Definition    


A. Component Helper - Create component helper folder with below two classes,

        1. Base Page - Create constructor of class & initialize the webdriver instance using the driver reference & below custom reusable functions created to perform actions on web element

        a. enterText            - Enter value on text box using "Send keys" method

        b. waitAndClick         - Perform click operation on web element using "Click" method e.g. button,Link

        c. ExecuteScript        - To scroll on webelement on page using "IJavaScriptExecutor"

        d. ScrollToAndClick     - Scroll & click on web element on page based on Location Y/X

        e. clickBasedOnText     - Click on web elements(Button, Links) using "Click" method based on index for more than one matching elements on page.

        f. selectDropDownValue  - Select drop down value using "Click" method based on index for more than one matching elements on page.

        g. IsElementVisible     - Verify element is present

        h. IsElemetPresent      - Verify element is present

        i. getAllTableValues    - Display tables values based on Row & Column count

        j. getRowCount          - Get table row count

        k. getColumnCount       - Get Column count

        l. getTextsTableResult  - Display tables values

        m. AreEqual             - To compare Actual Vs Expected

        2. DriverFactory - Initilize the driver object for Chrome & Edge browser & launch browser based on the AppConfigKeys

B. Configuration - Create Configuration folder with the below details,

1. App.Config - This file we have the configuration details for the,

                a. SpecFlow & .Net Framework
               
                b. app settings
               
C. Features - Reference of all BDD feature files & feature file contains BDD scenario

D. Page Object - Create page object pages with the webelement locator

E. Settings - Framework pre-execution setting before run script,

              1. AppConfigKeys - Before run script specify the browser name which we want to launch browser e.g. chrome/Edge & application URL.

F. Step Definition - This file we have the BDD step definition code
