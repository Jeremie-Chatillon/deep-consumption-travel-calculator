# deep-consumption-travel-calculator

<!--idée de nom n°2: deep-gray-energy-calculator--> 



## Overwiew

The main goal of this application is to create a calculator who gonna compute all the gray energy to create and to deliver some food. The users would be able to crate a earth between two localizations and the app will calculate the energy needed. It will be possible to add the product "creation energy cost" for some localization.

 This is to respond to the question: **"Is it better to consume local or something produced in a other country in best condition."**
The second goal is to create a community of developers and customers who care about ecology and want to share them knowledges. That is why it gonna be an open source project. Every body can make some improvement, correct some code or make some change proposals. The application's data gonna be provided by the users and cross-validated. <!-- créer un discord -->

The last goal is more personnel. I want is to use my IT competences to create a project, discover new technologies and improve myself. The technologies surely would not be the bests or the most use. However, the gonna teach me something and be open source to fit with the second objective.

​	

## Software development approach

The development approach is an adaptation of the **Agile** method. The app's creation will be spitted into different parts more or less independent. The project can be subject to changes. Every parts will be tested before to start a new functionality. *(Testing is mandatory then I'll try to do my best with this point with no guaranties.)*
At the beginning of an new project parts, I will plan a milestones to give me a time objective. *(I do this project on my free time then milestones gonna motivate me to make this project without too much procrastination.)*





### Step 0: GitHub and Overview

Create a public Github repository for the project. Then crate the the overview documentation (this one). He contains the tenants and resulting of the project. 

The overview will be completed during all the project because it is for me a boring task and i prefer to pases a bit of time every day on it rather than take complete days on it. 

### Step 1: Rooting Map

This step is to create a web app to diplay a card on which the user can make some roots. The user can 

#### Objectives:

- The user can select a starting location.
- The user can add a way from the current location to a next location. The last location is the final (like a "linked list").
- The user can select a means of transport (boat, plane, driving, train) for each way.
- The transport distance will be displayed. 
  - The total distance.
  - One distance for each means of transport.

##### Time: 

It has to be finished on 1st August 2020. (one week should be enough to learn Vue.js and create a map)



### Step 2: Rooting Map validation

This step is to validate the rooting:

- Boats:
  - Have to start and end in a seaport (all seaport in a first time then only in the commercials).
  - Have to travel on navigable waters.
- Planes:
  - Have to start and end in a airport (all airport in a first time then only in the commercials).
- Driving: 
  - Have to follow valid roads.
- Trains:
  - Have to follow valid railway.

#### Step 3: Energy calculator

Calculate the energy needed to do the travel.  At this point, all means of transports will have their own generic calculator. The calculator will take the distance traveled and will calculate the Co2 needed. I will assume for the moment every means of transport need the same energy everywhere in the heart.

The computation take a weight (or maybe a size) of the product we want to root and will compute in function of the maximum wight capacity of the transports means. 

#### Step 4: UI improvement





## deep energy calculator



## Infrastructure

This gonna be a **webapp** with 3 logical tiers.



## Technologies

### Backend

Express ou Django

### BD

firebase simple



### front-end

##### framework



#####  **vue.js**

This has been chosen because:

- I wanted to discover this technology.
- It permits to do webapp without a back-end.
- It is a progressive framework (it can be use with otter framework).

##### web UI components

https://blog.bitsrc.io/11-vue-js-component-libraries-you-should-know-in-2018-3d35ad0ae37f

- Ant design
- vuetifyjs
- Vue Material Design

