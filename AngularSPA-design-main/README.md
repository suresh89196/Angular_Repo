# AngularSPA-design
AngularSPA Design

 (a) Angular7/8 test

1. Design a small Single Page Application(in Angular 7/8 ) to manage a list of people.

Create at least 3 views:

>>list all people

>> edit a person

>>delete a person

### Angular 7/8 People Management Application

 created a Single Page Application in Angular to manage a list of people with the three required views. Let's build this step by step.

```typescriptreact project="angular_people_management"
...
```

## How the Application Works

This Angular application provides a complete solution for managing a list of people with the three required views:

1. **List View** - Displays all people in a responsive table with options to edit or delete each person
2. **Edit View** - Allows editing an existing person's details with form validation
3. **Delete Functionality** - Implemented in the list view with a confirmation dialog


### Key Features

- **Responsive Design**: Works on mobile and desktop
- **Form Validation**: Ensures data integrity
- **Loading States**: Shows loading spinners during API calls
- **Error Handling**: Displays user-friendly error messages
- **Confirmation Dialogs**: Prevents accidental deletions


### Implementation Details

1. **Services**:

1. `PeopleService` handles all API calls using Angular's HttpClient
2. Implements proper error handling



2. **Components**:

1. `PeopleListComponent` displays all people and handles deletion
2. `PersonEditComponent` handles both adding and editing people
3. `NavbarComponent` provides navigation
4. `LoadingSpinnerComponent` shows loading state



3. **Routing**:

1. Configured to navigate between views
2. Handles URL parameters for editing specific people





### How to Use the API

The application is set up to work with a REST API. You'll need to update the `apiUrl` in the `PeopleService` to point to your actual API endpoint. The service is already configured to handle:

- GET requests to fetch all people or a single person
- POST requests to add a new person
- PUT requests to update an existing person
- DELETE requests to remove a person


## Next Steps

1. Update the API URL in the `PeopleService` to point to your actual REST API
2. Customize the Person model if your API uses different field names
3. Add additional features like sorting, filtering, or pagination if needed
