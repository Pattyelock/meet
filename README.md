# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

# Meet App - User Stories & Scenarios

## App Key Features  

### 1. Filter Events by City  

**User Story:**  
AS a user,  
I should be able to filter events by city,  
SO that I can see a list of events taking place in that city.  

**Scenarios:**  

- **Scenario 1:** When user hasn’t searched for a specific city, show upcoming events from all cities.  
  - **GIVEN** user hasn’t searched for any city;  
  - **WHEN** the user opens the app;  
  - **THEN** the user should see a list of upcoming events.  

- **Scenario 2:** User should see a list of suggestions when they search for a city.  
  - **GIVEN** the main page is open;  
  - **WHEN** user starts typing in the city textbox;  
  - **THEN** the user should receive a list of cities (suggestions) that match what they’ve typed.  

- **Scenario 3:** User can select a city from the suggested list.  
  - **GIVEN** user was typing “Berlin” in the city textbox AND the list of suggested cities is showing;  
  - **WHEN** the user selects a city (e.g., “Berlin, Germany”) from the list;  
  - **THEN** their city should be changed to that city (i.e., “Berlin, Germany”) AND the user should receive a list of upcoming events in that city.  

### 2. Show/Hide Event Details  

**User Story:**  
AS a user,  
I should be able to show or hide event details,  
SO they will not always be hidden or displayed.  

**Scenarios:**  

- **Scenario 1:** User wants to see event details by clicking a button.  
  - **GIVEN** user wanted to see event details;  
  - **WHEN** they click the "Show details" button;  
  - **THEN** the user should see more details about the event.  

- **Scenario 2:** User wants to hide event details by clicking a button.  
  - **GIVEN** user wanted to see less information about an event;  
  - **WHEN** they click the "Hide details" button;  
  - **THEN** details will be hidden.  

### 3. Specify Number of Events  

**User Story:**  
AS a user,  
I should be able to specify number of events,  
SO that the right amount of events will be displayed.  

**Scenarios:**  

- **Scenario 1:** User wants to specify how many events they want to see.  
  - **GIVEN** user specified a number of events;  
  - **WHEN** searching for events;  
  - **THEN** the right amount of events will be displayed.  

- **Scenario 2:** User didn't provide a number of events to display.  
  - **GIVEN** user didn't provide a number;  
  - **WHEN** they searched for events;  
  - **THEN** all events meeting other criteria should be displayed.  

### 4. Use the App When Offline  

**User Story:**  
AS a user,  
I want to use the app offline,  
SO the app is available without an internet connection.  

**Scenario:**  
- **GIVEN** user could store the current state of the app on their device;  
- **WHEN** they have access to the internet;  
- **THEN** the user will be able to use the stored state of the app.  

### 5. Add an App Shortcut to the Home Screen  

**User Story:**  
AS a user,  
I can add an app shortcut to the home screen,  
SO I can access the app quickly.  

(This feature depends on system functionality and cannot be tested programmatically.)  

### 6. Display Charts Visualizing Event Details  

**User Story:**  
AS a user,  
I can view charts visualizing event details,  
SO I can easily understand the event data.  

**Scenarios:**  

- **Scenario 1:**  
  - **GIVEN** I am on the event details page;  
  - **WHEN** I view the event details;  
  - **THEN** I should see a chart visualizing the event data.  

- **Scenario 2:**  
  - **GIVEN** I have selected a specific event;  
  - **WHEN** I navigate to the event details page;  
  - **THEN** I should see a chart that displays the event's data in a visual format.  
