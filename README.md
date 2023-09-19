Study App README
Overview
This README provides an overview of the MainWindow.xaml.cs code for a simple Study App implemented in C# using the Windows Presentation Foundation (WPF) framework. The application allows users to input information about a course, such as course name, code, credits, class hours, self-study hours, and semester, and then calculates the recommended weekly study hours.

Code Description
Here's a breakdown of the key components and functionality of the code:

Namespaces

The code begins by importing several namespaces necessary for WPF and basic C# functionality.
MainWindow Class

This class represents the main window of the application and contains event handlers and methods for its functionality.
MainWindow Constructor

The MainWindow constructor initializes the main window when the application is started. It calls the InitializeComponent() method to set up the window's visual components.
Event Handlers

The code defines event handlers for various UI elements, such as buttons and text boxes.

TextBox_TextChanged: An event handler for text box changes (not currently implemented).

Button_Click: Closes the application when a specific button is clicked.

Button_Click_1: Clears the content of several text boxes when another button is clicked.

Button_Click_2: Performs calculations when a button is clicked. It extracts input data from text boxes (course name, code, credits, class hours, self-study hours, and semester), performs calculations, and displays the result in a text box.

Calculation Logic

Inside the Button_Click_2 event handler, the code extracts input values, multiplies credits by a constant (Multiply), calculates recommended weekly study hours based on the number of credits and semesters, and subtracts class hours to obtain the recommended self-study hours.
UI Components

The UI components are defined in the associated XAML file (MainWindow.xaml) and include text boxes (Box1, Box2, Box3, etc.) for input and a text box (Box8) for displaying the calculated result.
How to Use
Launch the application.
Enter the course information in the appropriate text boxes: course name, code, credits, class hours, self-study hours, and semester.
Click the "Calculate" button (Button_Click_2) to calculate the recommended weekly study hours.
The result will be displayed in the Box8 text box.
You can also use the "Clear" button (Button_Click_1) to clear the input fields if needed.
To exit the application, click the "Close" button (Button_Click).
Dependencies
The code relies on the Windows Presentation Foundation (WPF) framework and the associated libraries for creating the graphical user interface (GUI) of the application.
