# Online Booking System - Client

## Flux Architecture
#### Key Components
1. Actions - Represent events or interactions that occur wthin the application.
             JavaScript objects with a `type` property that describe the type of action.

2. Dispatcher - Responsible for managing for the flow of data within the application.
                It receives actions and dispatches them to registered stores.

3. Stores - Contain the application's state and business logic. They respond to actions and
            dispatched by the Dispatcher, update their state, and eit change events.
            Only entities in Flux that can hold the application's state.

4. Views (React Components) - Responsible for rendering the user interface based on the data provided
                              by stores. When the store's state changes, views are notified, and they
                              re-render to reflect the updated data.


## Architecture - Unidirectional Data Flow
The flux architecture follows a unidirectional data flow:
  * A user interacts with a view, triggering an action
  * The action is sent to the Dispatcher
  * The Dispatcher notifies registered stores
  * Stores update their state in response to the action
  * Stores emit change events
  * Views (React components) listen for change events and update their presentation based on the new
    state from the stores

This predictable flow of data makes it easier to understand and maintain the application as it grows.


## Getting Started
To run the project locally, follow these steps:
  1. Clone the repository: `git clone https://github.com/your-username/Backend-System-Client.git`
     Should you prefer to use personal access token: git clone https://<access toke>/github.com/your-username/Backend-System-Client.git
  2. Navigate to the prokect folder: `cd Booking-System-Client`
  3. Install dependencies: `npm install`
  4. RUn the development server: `npm run dev`
  5. Open your browser and visit: `http://localhost:3000`


## License
This project is licensed under the MIT License - see the LICENSE.md file for details.-


