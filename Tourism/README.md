# Launch Mod 3 Week 2 Assessment

## Questions (10 Points)

1. Define MVC and explain the purpose of each of the three parts of this pattern.
- **Model** - Handles state and business logic; How data may be shown created, stored, and altered
- **View** - The actual look of the user interface; no business logic should take place here
- **Controller** - The controller handles user interaction; responding to it when needed.
2. Explain the difference between the **New** route and the **Create** route.
</br>The **New** route offers a form to create a new object.
</br>The **Create** route creates the new object on the server.
3. List all of the RESTful routes for the `employee` entity. Make sure to include the Route Name, Path, and HTTP Method for each of the routes. (2 points)
</br>
| Route Name | Path               | Http Method | Purpose                                   |
|------------|--------------------|-------------|-------------------------------------------|
| Index      | /employee          | GET         | displays all employees                    |
| New        | /employee/new      | GET         | form for creating new employees           |
| Create     | /employee          | POST        | creates the new employee on the server    |
| Show       | /employee/:id      | GET         | displays one employee's details           |
| Edit       | /employee/:id/edit | GET         | offers form to edit an employee's details |
| Update     | /employee/:id      | PATCH       | updates the employee's details on server  |
| destroy    | /employee/:id      | DELETE      | deletes the specific employee             |
</br>
For the following three questions, explain both how to fix the error/bug and why the part of the code that was broken is important. (2 points each)

4. The variable hotels in the Index() method of the HotelsController needs to be passed as an argument to View() when it is returned. 
<img width="1213" alt="Screenshot 2023-06-13 102204" src="https://github.com/turingschool/launch-curriculum/assets/11747682/f37c233d-e7aa-483e-9f75-7c9b111811e5">


5. The view for Index() is named improperly, It looks to be called Indexes.cshtml in the solution explorer under the folder Hotels.
<img width="1245" alt="Screenshot 2023-06-13 102555" src="https://github.com/turingschool/launch-curriculum/assets/11747682/87c9fbf7-de63-4580-9b36-8632df27b91b">

6. To properly display C# variables in the view the variable must be prefixed with an @ symbol. (ex: @hotel.Name, @hotel.Location)
<img width="1238" alt="Screenshot 2023-06-13 102856" src="https://github.com/turingschool/launch-curriculum/assets/11747682/a39b525d-ae05-463f-b724-be68aa70148c">

## Exercise (10 Points)

Make sure to first run `update-database` to populate the `Tourism` database used by this application.

This application already has the `Index` route for States.

Your task is to do the following:
1. Add the `Show` RESTful route to display the name and abbreviation for a particular state.
1. Add a test for your new `Show` route in the `StateCRUDTests.cs` file.
