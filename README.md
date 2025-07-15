# Selenium WebDriver Java Test Suite

This project is a Java-based automated test suite using Selenium WebDriver and TestNG/JUnit. It demonstrates a variety of browser automation techniques by testing against [the-internet.herokuapp.com](https://the-internet.herokuapp.com).

## Project Structure

- `src/main/java/` — Page objects and utility classes:
  - `pages/`: Page Object Model classes for each tested feature/page.
  - `utils/`: Helpers for cookies, window management, and event reporting.
- `src/test/java/` — Test classes organized by feature:
  - `Alerts/`, `dropdown/`, `frames/`, `hover/`, `login/`, `Navigation/`, `slider/`, `wait/`, etc.
  - `SimpleWebTest.java`: Example of a simple web search test.
- `resources/` — Contains:
  - `chromedriver.exe`: ChromeDriver binary for running tests.
  - `screenshots/`: Stores screenshots taken on test failures.

## Key Features & Test Coverage

- **Authentication:** Login and secure area tests
- **Alerts:** Handling JavaScript alerts, confirms, and prompts
- **File Upload:** Automated file upload tests
- **Dropdowns:** Selecting options from dropdown menus
- **Frames:** Interacting with frames and WYSIWYG editors
- **Hover:** Mouse hover actions and profile popups
- **JavaScript:** Executing scripts, infinite scroll, and dynamic content
- **Keyboard:** Simulating key presses
- **Navigation:** Browser navigation and window/tab management
- **Sliders:** Interacting with horizontal sliders
- **Dynamic Loading:** Waiting for elements to appear/disappear
- **Cookies:** Managing browser cookies
- **Waits:** Explicit and fluent waits for synchronization
- **Simple Web Test:** Example search on DuckDuckGo

## Utilities

- **CookieManager:** Add, delete, and check cookies
- **WindowManager:** Manage browser windows/tabs and navigation
- **EventReporter:** Logs browser events for debugging

## Setup & Requirements

- Java 17 or higher
- Maven
- Google Chrome browser
- ChromeDriver (included in `resources/`)

Dependencies are managed via `pom.xml`:
- Selenium WebDriver
- TestNG
- JUnit Jupiter
- SLF4J

## How to Run

1. Ensure Google Chrome is installed and compatible with the included ChromeDriver.
2. Clone this repository and navigate to the project root.
3. Run the tests with:
   ```
   mvn test
   ```
4. On test failure, screenshots will be saved in `resources/screenshots/`.

## Extending the Suite

- Add new page objects in `src/main/java/pages/`.
- Add new tests in `src/test/java/` under the appropriate feature folder.

---

This project is ideal for learning and demonstrating best practices in Selenium WebDriver automation with Java. 

🛠 Technologies & Tools
Java 17
Selenium WebDriver 4.12.1
TestNG 7.7.0
JUnit 4.12
Maven
ChromeDriver

