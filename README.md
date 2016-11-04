tut-11-04-todoApplication

 * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
<------------------------------------------- Simple TODO App ------------------------------------------->
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
 * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



- - - - - - - - - - - - - - - - - - - - - - - - - Languages - - - - - - - - - - - - - - - - - - - - - - -

This is an exercise to learn the fundamentals of programming using:
* SQLite
* JavaScript
* HTML
* CSS


- - - - - - - - - - - - - - - - - - - - - - - Components of Apps - - - - - - - - - - - - - - - - - - - - -
 
While learning these programming languages, I will also learn the parts that make up a web app:
* models
* views
* controllers
* assets
  - templates
  - stylesheets


 - - - - - - - - - - - - - - - - - - - - - - - Basic Functions - - - - - - - - - - - - - - - - - - - - - -

The TODO App will allow the user create, read, update, and destroy items (tasks & categories)


- - - - - - - - - - - - - - - - - - - - - - - - - Item Views - - - - - - - - - - - - - - - - - - - - - - -

A task item includes the following properties:
* id
* title
* description
* creationDate
* dueDate
* completed
* priorityRank


A category item includes the following properties:
* id
* title
* description

(Default categories: incomplete, completed, school, work, fitness)


- - - - - - - - - - - - - - - - - - - - - - - - User abilities - - - - - - - - - - - - - - - - - - - - - -

Events the user will be able to perform:

_1.___create new tasks or categories____________________________________________________________________ _
  - no matter what, certain properties should be set by the program itself
    - such as: id, creationDate, and complete (by default it should be false)
    
_2.___edit tasks/categories_____________________________________________________________________________ _
  - change properties of tasks or categories
    <<example:>> user should be able to modify the dueDate
    
_3.___view a collection of tasks________________________________________________________________________ _
  - by sorting tasks based on task properties
    - example: when sorted by creationDate
      - a task named "Run 30 min" created on Sep 8th, will come before "Finish Homework" created Sep 22nd
  - by filtering using categories assigned to tasks
    <<example:>> when sorted by category { title: "complete" }
      - only task items with boolean property "completed" set to true will be shown

```js
  if (task.completed == true) {
    view.collection.each( function(category) { 
      category.title("complete")
    });
  }
```


- - - - - - - - - - - - - - - - - - - - - - - Future Enhancements - - - - - - - - - - - - - - - - - - - -

!! Arrange items by time to complete !!
  - items should be viewable while category, "Time To Complete" is the rendered and shown in view.

!! designed to be a mobile first application !!
  - make it viewable on small resolutions

User can create tasks by using elements field inputs, dropdowns, and a calendar. he user can create, read, update, and destroy tasks.
