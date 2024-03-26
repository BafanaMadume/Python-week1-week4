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
