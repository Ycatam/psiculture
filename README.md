# Psiculture

This project have an objective, from an academic point of view, progressively implement an web application inpired in a psiculture environment. Where, at the end of the project, we'll be able to perform a registry of a fish poll data, having temperature, PH, portion, date and the day time of the measurement. Also, we will be able to edit, read and exclud the register.

The frontend of this application was developed with Angular, and the backend is simulated using JSON server.

## Deploy Address - GitHub Pages

https://ycatam.github.io/psiculture/

## Figma Prototype

https://www.figma.com/file/K9e1o9kU0nEe6lPSSatw9Y/psiculture?type=design&mode=design&t=43VTwL2ZzyrgB4ya-1

## Checklist

- [x] Create a Github repository with the gitflow structure, including at least the branch "main" and "develop.
- [x] Use a component of a CSS framework, like Bootstrap, Marterialize or other of your choise.
- [x] Uses responsive layout in the app screens, automatic adjusting for diferents screens sizes, using a CSS framework or with personalized implementations.
- [x] Develop the application layout using components, turning the header and the baseboard components that can be reused accross the application.
- [x] Apply at least two types of data-binding, like Interpolation, Property Binding, Event Binding, Two-Way Data Binding. 
- [x] Use template variables and ViewChild anottations to interact with DOM elements or components directly on the template or on the TypeScript code of the application.
- [x] Establish the passage of data between components through the component hierarchy, using the @Input and @Output annotations.
- [x] Transfer data, through services, between components that are not directly related.
- [x] Map components to routes in the routes module, creating an efficient navigation structure.
- [x] Allow fluid navigation between different application pages through navigation links and buttons.
- [ ] Validate form fields with regular expressions (REGEX) and display error messages.
- [x] Implement masks on form fields when necessary to improve the user experience when entering data.
- [x] Disable the submit button while the form is in an invalid state.
- [ ] Make API requests with appropriate handling of success and error responses with Promises.
- [x] Make API requests with appropriate handling of success and error responses with Observables.
- [x] Create the complete registration of an entity, including create, read, update and delete (CRUD) operations using an API, such as JSON Server.
- [ ] Use local storage (LocalStorage or SessionStorage) to store temporary data when necessary.
- [x] Apply the ngFor structural directive to present a dynamic list of data in your application.
- [x] Use the ngIf directive to control the showing or hiding of elements based on specific conditions.
- [x] Format the data presentation with Pipes, according to the application requirements.
- [x] Run the application build process and deploy it to make the application accessible online.

## Execution Manual
- Clone the repository with the command `git clone`
- Checkout to the branch `develop` which has the most recent versions
- Open the project with Visual Studio Code editor (VS Code)
- open an terminal from VSCode or any terminal on your Operating System pointing to the project root directory
- Install the dependencies contained in `package.json`
  - Coomand: `npm i`
- (Optional) Install the JSON Server `https://www.npmjs.com/package/json-server`
  - Command: `npm i -g json-server` 
  - It is optional because the dependency is already registered in the `package.json` file for local installation in the `node_modules` folder
- Run the Fake API (JSON Server) via one of the following commands: 
  - Execution via script registered in `package.json`: `npm run json:server:routes` 
  - Or via Explicit Execution: `json-server --watch db.json --routes routes.json`
- The command to execute JSON Server must be applied to the project's root directory, that is, the directory containing the file `db.json` and `routes.json`.
  - By default, the JSON Server application runs at the address `localhost:3000`    
- Open a new terminal in VSCode and then run the Angular project
  - Command: `ng s -o`