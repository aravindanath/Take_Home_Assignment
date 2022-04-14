# Webdriver Tests
## Prerequisites
  + Git (optional)
  - Java
  * Webdriver
  + ChromeDriver
  * IDE such as IntelliJ or Eclipse

## Steps
  
1. Set the following BaseUrl for your tests:

   `https://the-internet.herokuapp.com`
   
2. Use ChromeDriver to write Tests for the following scenarios in Java:
    * Login Success: https://the-internet.herokuapp.com/login credentials: tomsmith/SuperSecretPassword!
    + Login Failure: https://the-internet.herokuapp.com/login Login fail invalid creadentials
    - CheckBoxes: https://the-internet.herokuapp.com/checkboxes Check and uncheck boxes
    * ContextMenu: https://the-internet.herokuapp.com/context_menu Right-click in the box to see one called 'the-internet'. Test JavaScript alert text on Right-Click.
    + Drag and Drop: https://the-internet.herokuapp.com/drag_and_drop Perofrm Drag And Drop in a Webdriver test.
    - Dropdown: https://the-internet.herokuapp.com/dropdown Test dropdown using Webdriver.
    * Dynamic Content: https://the-internet.herokuapp.com/dynamic_content Test content changes with page reload.
    + Dynamic Controls: https://the-internet.herokuapp.com/dynamic_controls Test Dynamic Controls using Explicit Waits.
    - Dynamic Loading: https://the-internet.herokuapp.com/dynamic_loading/2 Test Dynamic Loading using Explict Waits.
    * File Download: https://the-internet.herokuapp.com/download Test File Download.
    + File Upload: https://the-internet.herokuapp.com/upload Test File Upload.
    - Floating Menu: https://the-internet.herokuapp.com/floating_menu Test Floating Menu.
    * Iframe: https://the-internet.herokuapp.com/iframe Test iframe.
    + Mouse Hover: https://the-internet.herokuapp.com/hovers Test Mouse Hover.
    - JavaScript Alerts: https://the-internet.herokuapp.com/javascript_alerts Test confirm JS Alert.
    * JavaScript Error: https://the-internet.herokuapp.com/javascript_error Test JS error.
    + Open in New Tab: https://the-internet.herokuapp.com/windows Test Link Opens in new tab.
    - Notification Message: https://the-internet.herokuapp.com/notification_message_rendered Test notification Message.
  
  
  
## Submission Rubrics

### General Requirements
1. All tests should contain @Test annotation.
2. All tests should provide a setup and tear down mechanism that closes the browser.
3. All tests should run successfully from IDE. 


### Test Specific Rubrics

1. Login Success
   * Page Object Model for the login page should be provided.
   + Test is able to login successfully.
   - Test uses an assertion to make sure User has logged in.

2. Login Failure
   * Page Object Model for the login page should be used.
   + Test is not able to login with wrong credentials.
   - Test uses assertions to check Login failed for incorrect user and password.

3. Checkboxes
   * Test checks and unchecks checkboxes.
   + Test uses assertions to make sure boxes were properly checked and unchecked.
4. Context Menu
   * Test right clicks on the context menu.
   + Test asserts the alert menu text.
5. Drag and Drop
   * Test drags element A to element B.
   + Test asserts that the text on element A and B are switched.
6. Dropdown
   * Test selects Option 1 and Option 2 from the drop down menu.
   + Test asserts Option 1 and Option 2 are selected.
7. Dynamic Content
   * Test refreshes the page a couple of times.
   + Test asserts that the content changes on each refresh.
8. Dynamic Controls
   * Test clicks on the Remove Button and uses explicit wait.
   + Test asserts that the checkbox is gone.
   - Test clicks on Add Button and uses explicit wait.
   * Test asserts that the checkbox is present.
   + Test clicks on the Enable Button and uses explicit wait.
   * Test asserts that the text box is enabled.
   + Test clicks on the Disable Button and uses explicit wait.
   - Test asserts that the text box is disabled.
9. Dynamic Loading
   * Test clicks the start button and uses explicit wait.
   + Test asserts that “Hello World!” text is displayed.
10. File Download
    * Test clicks on the file.
    + Test asserts that the file is downloaded.
11. File Upload
    * Test uses Upload Button or Drag and Drop to upload a file.
    + Test asserts that the file is uploaded.
12. Floating Menu
    * Test scrolls the page.
    + Test asserts that the floating menu is still displayed.
13. Iframe
    * Test switches to Iframe and types some text.
    + Test asserts that the typed text is as expected.
14. Mouse Hover
    * Test does a mouse hover on each image.
    + Test asserts that additional information is displayed for each image.
15. JavaScript Alerts
    * Test Clicks on JS Alert Button.
    + Test asserts alert message.
    - Test clicks on JS confirm Button and clicks ok on alert.
    * Test asserts the alert message.
    + Test clicks on JS Prompt Button and types a message on Prompt.
    - Test asserts that the alert message contains the typed message.
16. JavaScript Error
    * Test finds the JavaScript error on the page.
    + Test asserts that the page contains error: Cannot read property 'xyz' of undefined.
17. Open in New Tab
    * Test clicks on the Click Here link.
    + Test asserts that a new tab is opened with text New Window.
18. Notification Message
    * Test clicks on the Click Here link a multiple times.
    + Test asserts that one of the “Action Successful”, “Action unsuccessful, please try again” and “Action Unsuccessful” messages show on click.

 
