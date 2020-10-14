# deep-consumption-travel-calculator

<!--idée de nom n°2: deep-gray-energy-calculator--> 



## Overview

The main goal of this application is to create a calculator who gonna computes all the gray energy to create and to deliver some food. The users would be able to create an earth between two localizations and the app will calculate the energy needed. It will be possible to add the product "creation energy cost" for some localization. This is to respond to the question:**"Is it better to consume local or something produced in another country with better production conditions?"**

The second goal is to create a community of developers and customers who care about ecology and want to share them knowledges. That is why it gonna be an open source project. Everybody can make some improvement, correct some code or make some change proposals. The application's data gonna be provided by the users and cross-validated. <!-- créer un discord -->

The last goal is more personal. I want is to use my IT competences to create a project, discover new technologies and improve myself. The technologies surely would not be the bests or the most use. However, the gonna teaches me something and be open source to fit with the second objective.

​	

## Software development approach

The development approach is an adaptation of the **Agile** method. The app's creation will be supported into different parts more or less independent. The project can be subject to changes. Every parts will be tested before to start a new functionality. *(Testing is mandatory, then I'll try to do my best with this point with no guarantees.)* 
At the beginning of a new project part, I will plan a milestones to give me a time objective. *(I do this project on my free time, then milestones gonna motivate me to make this project without too much procrastination.)*



### Step 0: GitHub and Overview

Create a public Github repository for the project. Then crate the overview documentation (this one). He contains the tenants and resulting from the project.
The overview will be completed during all the project because it is for me a boring task and I prefer to pass a bit of time every day on it rather than take complete days on it.

### Step 1: Rooting Map

This step is to create a web app to display a card on which the user can make some roots.

#### Objectives:

- The user can select a starting location.
- The user can add a way from the current location to a next location. The last location is the final (like a "linked list").
- The user can select a means of transport (boat, plane, driving, train) for each way.
- The transport distance will be displayed. 
  - The total distance.
  - One distance for each means of transport.



### Step 2: Rooting Map validation

This step is to validate the rooting:

- Boats:
  - Have to start and end in a seaport (all seaports in a first time, then only in the commercials).
  - Have to travel on navigable waters.
- Planes:
  - Have to start and end in a airport (all seaports in a first time, then only in the commercials).
- Driving: 
  - Have to follow valid roads.
- Trains:
  - Have to follow valid railway.

#### Step 3: Energy calculator

Calculate the energy needed to do the travel. At this point, all means of transports will have their own generic calculator. The calculator will take the distance traveled and will calculate the Co2 needed. I will assume for the moment, every means of transport need the same energy everywhere in the heart.

The computation takes a weight (or maybe a size) of the product we want to root and will compute in function of the maximum weight capacity of the transports means.

#### Step 4: UI improvement





## deep energy calculator



## Infrastructure

For the two frist steps, no backend is needed. Then I would go do a 3tiers  architecture and a **RestAPI** to communicate between the backend and the frontend.



## Technologies

### Backend

Express ou Django

### DB

firebase simple



### front-end

##### framework

Vue.js

#### Linter

Eslint

​	`yarn add -D eslint eslint-plugin-vue@next`



#####  **vue.js**

This has been chosen because:

- I wanted to discover this technology.
- It permits to do web app without a back-end.
- It is a progressive framework (it can be used with other framework).

##### web UI components

https://blog.bitsrc.io/11-vue-js-component-libraries-you-should-know-in-2018-3d35ad0ae37f

Multiples choices:

- Ant design
- vuetifyjs
- Vue Material Design
- Element

I will use **ElementUI** because it is well documentEd and many people recommend it to me.

