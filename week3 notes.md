# Python week 3
## Intermediate Python

1. Project planning
2. Content Retrieval
3. Digest email
4. Building a Graphical User Interface (GUI)
5. Design iteration
6. Project Packaging and Distribution

## PROJECT PLANNING
### FINDING INSPIRATION
First thing to solve when embarking on a new programming endeavour for enjoyment or practice,is the initial puzzle to solve:
What should the program accomplish ?.first step is to seek inspiration from what you love ,such as hobbies or a problem you would want to solve.
* workspace can also serve as a wellspring of ideas ,also checking if the aspects of your job is what could benefit from automotion?
* * Also Reflecting on task that can be done through automation

### USER STORIES
User stories depict small scenarios from a users perspective.they should emphasize the user's goal and motivation rather than the application itself
* USER STORIES are :
  - Brief
  - simple
  - informal
  - perfect for jotting down on index cards
* They follow a Format
  - As a [user/role],
  - i want [goal],
  - so that [reason/benefit]
 
* Why User Stories are Important:

* Focus on Users: By keeping the user's perspective central, user stories ensure the application is designed to meet their needs and goals.
* Improved Communication: The simple format fosters clear communication between developers, designers, and product owners.
* Flexibility: User stories are adaptable. As projects evolve, user stories can be easily modified to reflect new requirements.Additional Tips for Writing User Stories:

* Use Active Voice: Structure the story as "As a [user], I want [goal]" for clarity and focus. One Story, One Goal: Keep each user story centered around a single user goal for better understanding and development.
* Measurable Value: Whenever possible, frame the reason/benefit in a measurable way (e.g., "reduce errors by 50%").
  
### Examples of User Stories:

E-commerce Website:
As a customer, I want to search for products by category and brand so that I can easily find what I'm looking for.
As a customer, I want to see reviews from other customers before I buy a product so that I can make informed decisions.
Mobile Banking App:
As an account holder, I want to be able to check my account balance quickly and easily so that I can manage my finances on the go.
As a bill payer, I want to schedule automatic payments for my bills so that I never miss a due date.

 ![figure3](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/17fb3b3a-408f-431c-adbe-b85c5e81cc0b)

* What to remember when writing user stories,focus on the user's goals and reasons,rather than specific interface details or implementation methods.

 ### USE CASES
 * use cases Typically include a title ,an actor (a user or system) and a scenario that describes how a goal is achieved
 * The scnario can be written as a paragraph or a list of steps in simple language .E.g use case may involve a digest recipient reading tweets on a specific twitter trend by opening the email,clicking on the trend link and accessing the corresponding twitter page.
 * use cases ,they capture different information ,user stories focus on the **Who,what and how of achieving that goal**.
   

 ![figure4](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/7150faa6-de87-466a-963d-616f4fa2c5b7)
 ![figure 5](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/ac3be55c-2dab-4ff8-9cdb-d992d27da9a6)

 ### Project Requirements
 It is helpful to write traditional requirements to formally capture the capabilities and limitations of an application.
 * Functional requirements describe what the application should or should not do and are written as sentences starting with the **The aplication must or The application shall**
 * ![figure6](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/3783951d-958b-48ea-bada-21a391b77324)

* These requirements are kept at a high level whereby omitting specific details such as the forecast duration or temperature unit.For personal projects ,this level of detail suffices and elaboration can be left for implementation
* Functional requirements related to the admin include configuring content sources ,adding and removing recipients ,scheduling the email digest and setting email account credentials
* Non -Functional requirements describe how the application should accomplish its tasks.
  - They focus on qualities like
      - Maintainability
      - reliability
      - usability
   
### ARCHITECTURE
since our requirements are captured,we need to organize and structure the code for presentation purposes,since python is an object oriented programming language,considering objects and classes is essential
* BY looking at the requirements,use cases and user stories , identifying nouns helps determine potential objects
* In functional requirements words like:
  - quote
  - forecast
  - location
  - trends
  - article
  - content
  - email
  - recipients
* Grouping together related nouns such as content and emails provides a starting point for potential classes.
* Content class is responsible for generating and retrieving content
* email class handles formatting content and sending emails,
* GUI class manages configuration- related behaviours
  BY doing this the process helps draft method names and provides an initial structure for the program
  GUI =  Graphical User Interface. It's the way you interact with most electronic devices
        
![figure7](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/c5d264ee-3f8d-4b87-b4cb-502d9af49621)

* Grouping related nouns together such as content and email,provides a starting point for potential classes.Content email,and Gui emerge as candidate for classes,the behaviours and responsiblities are determined by extracting simplified verb phrases from requirements.

![figure8](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/8fa87fef-7afb-46d0-838a-fe8b5d5cd695)

## Stub code
python modules : dd_content.py,dd_email.py,dd_gui.py

## dd_email.py
![dd_email](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/f8b391bd-2470-41f1-8f14-a0620a60b1ed)

this code defines a class called `DailyDigitalEmail` that likely represents an email notification system.

**Class Definition:**

* `class DailyDigitalEmail:`: This line defines a new class named `DailyDigitalEmail`. Classes are blueprints for creating objects that share similar properties and behaviors.

**Class Methods:**

* `def __init__(self) :`: This is a special method called the constructor. It's automatically called whenever you create a new instance (object) of the `DailyDigitalEmail` class. In this case, the constructor is empty (`pass`), but it can be used to initialize any default values or configurations for the email object.
* `def send_email(self):`: This method likely handles sending the actual email notification. It presumably takes care of composing the email message, specifying recipients, and utilizing an email service to deliver it. However, the code doesn't show the implementation details of how the email is sent.
* `def format_message(self):`: This method is probably responsible for formatting the content of the email message. It might involve creating the email body, including text, images, or attachments. Similar to `send_email`, the specific formatting logic isn't provided in this code snippet.

**Main Block:**

* **if __name__ == '__main__':**`: This block is used to encapsulate code that should only run when the script is executed directly (not imported as a module). It's currently empty (`pass`), but typically this section would contain test code to verify the functionality of the class methods. 

## dd_content
![dd_content](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/fa9782e5-7b83-4e93-9032-cc8b352a1984)

This code defines several functions that likely retrieve information for a daily digital email.

* `def get_random_quote():`: This function presumably fetches a random inspirational quote or saying. It might achieve this by accessing a website or online database that provides quotes. 
* `def get_weather_forecast():`: This function likely retrieves the weather forecast for a particular location. It could involve interacting with a weather API (Application Programming Interface) to get the forecast data.
* `def get_twitter_trends():`: This function  probably fetches the current trending topics on Twitter. It might necessitate utilizing the Twitter API to access this information.
* `def get_wikipedia_article():`: This function  presumably retrieves a Wikipedia article, possibly based on a random topic or a pre-defined selection. It could involve interacting with the Wikipedia API to search and retrieve the article content.

**Main Block:**

* `if __name__ == '__main__':`: Similar to the previous code, this block is for test purposes. Here, it's empty (`pass`), but ideally, it would contain code to call each function and potentially display or process the retrieved information (quotes, weather, trends, articles).

## dd_GUI
![dd_gui](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/fdacf890-d096-4c94-803c-743277a36226)

 This code defines a graphical user interface (GUI) class using Python's Tkinter library. Let's break it down:

**Import Statements:**

* `from tkinter import*`: This line imports everything from the Tkinter library, providing all the widgets and functionalities needed to build the GUI.
* `from tkinter import ttk`: This line imports the `ttk` submodule from Tkinter, which offers additional widgets with a more modern look and feel.

**Class Definition:**

* `class DailyDigestGUI:`: This defines a class named `DailyDigestGUI` responsible for creating the visual elements of the daily digest application.

**Class Constructor:**

* `def __init__(self,root):`: This is the constructor method that gets called whenever you create a new instance of `DailyDigestGUI`. It takes a `root` parameter, which likely represents the main application window. Here, the constructor is empty (`pass`), but typically it would be used to add GUI elements (widgets) to the `root` window.

**Main Block:**

* `if __name__ == '__main__':`: This block ensures the code within it only executes when the script is run directly (not imported as a module).
* `root = Tk()`: This line creates the main application window using the `Tk()` constructor from Tkinter.
* `app= DailyDigestGUI(root)`: This line creates an instance of the `DailyDigestGUI` class, passing the `root` window as an argument to the constructor. This likely triggers the building of the GUI within the `__init__` method.
* `root.mainloop()`: This line starts the main event loop for the Tkinter application. It listens for user interactions (button clicks, etc.) and updates the GUI accordingly.

this code sets up the foundation for a daily digest GUI application using Tkinter. The `DailyDigestGUI` class is likely intended to be filled with code to add various UI components like labels, buttons, and potentially text boxes to display the retrieved content (quotes, weather, trends, articles) from the previous code snippet. 

### Summary on tkinter
Tkinter is a Python library that allows you to create graphical user interfaces (GUIs) for your desktop applications. It's considered the **de facto standard GUI library for Python** because it's:

  * **Built-in:** Tkinter comes pre-installed with most Python distributions, so you don't need to download any additional libraries to use it.
  * **Cross-platform:**  The same Tkinter code can run on Windows, macOS, and Linux with minimal changes, making it versatile for developing applications that work across different operating systems.
  * **Simple to learn:** Tkinter offers a relatively easy-to-learn API (Application Programming Interface)  compared to other GUI libraries in Python. 

Here's a deeper dive into Tkinter:

**Key Concepts:**

* **Widgets:** Tkinter provides a set of pre-built graphical components called widgets. These include buttons, labels, text boxes, frames, menus, and more. You can arrange and configure these widgets to create the visual layout of your application.
* **Event-driven programming:** Tkinter applications are event-driven. This means the program waits for user interactions (like mouse clicks or key presses) and then executes the corresponding code based on those events.
* **Object-oriented:** Tkinter utilizes an object-oriented approach. Each widget is represented as an object with its own properties and methods. You can create and manipulate these objects to build your GUI.

**Benefits of using Tkinter:**

* **Rapid prototyping:** Tkinter's simplicity makes it a good choice for quickly creating prototypes of your application's user interface.
* **Lightweight:** Tkinter applications tend to be lightweight and have a smaller footprint compared to some other GUI libraries.
* **Easy integration with Python:**  Since Tkinter is built into Python, it integrates seamlessly with the language, allowing you to leverage Python's rich functionality within your GUI application.

**Here are some limitations to consider:**

* **Basic look and feel:** Tkinter's default widgets can appear somewhat outdated compared to more modern GUI libraries. However, there are ways to customize the appearance with themes or third-party extensions.
* **Limited advanced features:** While Tkinter covers the essential GUI elements, it might lack some advanced features available in other libraries, such as drag-and-drop functionality or complex animations.

**Learning Resources:**

 learning more about Tkinter, here are some helpful resources:

* **Official Tkinter documentation:** [https://docs.python.org/3/library/tk.html](https://docs.python.org/3/library/tk.html)
* **Real Python Tkinter Tutorial:** [https://realpython.com/tutorials/gui/](https://realpython.com/tutorials/gui/)
* **Python GUI Programming with Tkinter book:** [https://nostarch.com/catalog/python](https://nostarch.com/catalog/python)

Questions 
* 1. what is the recommended approach for crafting a standard user story?
     - = Describe a single scenario from th user's perspective.
* 2. What is the description of the question that nonfunctional requirements need to address for an application
     - = "how should it do something
* 3. How can you  begin to determine what classes you will need for your python app?
