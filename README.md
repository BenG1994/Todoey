# Todoey

Todoey is a todo list app that allows you to create different categories for you items, as well as delete them when you are done instead of simply checking them off.

## Introduction

Todoey is from a tutorial by Angelu Yu with the focus on working with tableviews, saving data with both CoreData and Realm, along with implementing SwipeCellKit to delete items from tables.

## Skills used

* TableViews, checkmarks for cells
* CoreData
* Realm
* Embed in navigation view
* SwipeCellKit - Swift Package

## Process and challenges

While the main structure of creating the app was following the tutorial, I learned some interesting things along the way, mostly with tableviews. As those are one of the most common tools used in iOS, it was good to gain a strong understanding of how those work and how to use them. The app showed how to link two of them together with a DataModel using CoreData, which was later replaced by Realm as a way to save and write a database for all the categories and items in each category for your todo items.

![Simulator Screen Recording - iPhone 14 Pro - 2023-02-06 at 10 48 22](https://user-images.githubusercontent.com/113778995/217033604-35d686da-5bd3-4f06-9eff-a279a99bbb19.gif)                  ![Simulator Screen Recording - iPhone 14 Pro - 2023-02-06 at 10 48 48](https://user-images.githubusercontent.com/113778995/217033624-fd09b881-6753-4066-b7d0-0cdff4ce6608.gif)


I like that it offered two different ways of saving user data from the tables as some options are better than others in different situations. I chose to rewrite everything in Realm as it was less code and more straightforward for an instance like this where it only saved 3-4 properties to each item.

In addition to adding categories for items, users can also search through all the items in a certain category. That will limit the number of items show in the tableview to just their search text. Once a user clears the search bar, all the original items in the table return to normal.

![Simulator Screen Recording - iPhone 14 Pro - 2023-02-06 at 10 49 49](https://user-images.githubusercontent.com/113778995/217033690-7aeb7f3a-b843-4697-a79c-50310514b2c8.gif)

After all the tableviews and search options were completely, a package was added to the project to delete cells on a swipe action. SwipeCellKit allow me to create that action very simply, with the ability to customize how it looked, how long it took, and if there were other options than just deleting the cell. 

![Simulator Screen Recording - iPhone 14 Pro - 2023-02-06 at 10 49 03](https://user-images.githubusercontent.com/113778995/217034027-6e64b2cf-26c6-4c9f-b711-79cf6c9056b3.gif)

## Reflection

While the tools learned in this tutorial weren't overly complex, they are extremely well-used. It was important to learn these skills early on and see how they can be implement in different ways and use other tools to help improve the experience opposed to using the base tableview cells. 
