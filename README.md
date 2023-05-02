# Hotel MVC: Into the Model-View-Controller (MVC) 
guided by H Grasso

This presentation provides a comprehensive overview of the Model-View-Controller (MVC) architecture, using creative analogies such as a hotel, to explain the roles of the Model, View, and Controller, along with additional components like Mongoose, routers, middleware, and databases, in building robust and scalable applications.

![Hotel MVC_ Into the Model-View-Controller](https://user-images.githubusercontent.com/119631464/235600806-5bb8fc38-5948-485b-b154-86947f129b00.svg)

Today is your first day working at the Luxurious HOTEL MVC! Sorry, you’re not staying there- Luckily, you are in for a treat because for your first day, we have something special planned: we are going to be talking about the Model-View-Controller (MVC) architecture! 

![Hotel MVC_ Into the Model-View-Controller (1)](https://user-images.githubusercontent.com/119631464/235600923-f2a8ca21-440b-41fe-a4d6-bb1f4801ae7d.svg)

So first, what is MVC? MVC is a software design pattern that separates an application's data, user interface, and control logic into three distinct components: the Model, the View, and the Controller.

To help us understand MVC better, we’ll be going on a tour through our MVC Hotel. As you can see, there's a bit more to just the Model, View, and Controller here. On our tour we will be taking a look at every part that makes our MVC run successfully: Our guests, our grand hallways, our front desk, our Model employees, our ledger, and our guest rooms. 

Oh look! And here are our guests now! Let’s greet them!

![Hotel MVC_ Into the Model-View-Controller (2)](https://user-images.githubusercontent.com/119631464/235600947-129a9e72-c0ce-41dd-ac1e-efa5b167b365.svg)

The browser can be likened to a guest who enters the hotel. 

*Oh, hello! Welcome!*

The browser is the software application that users interact with to access and navigate web pages. It acts as the medium through which users communicate with the MVC application, just as a guest interacts with the hotel staff and facilities. 

The browser sends requests to the server, receives responses, and displays the content to the user, much like how a guest interacts with the hotel staff to make requests and receives services. 

Let’s help them inside, shall we?

![Hotel MVC_ Into the Model-View-Controller (3)](https://user-images.githubusercontent.com/119631464/235600985-5ef9feed-4758-4cf6-8a9d-f093d1193b8a.svg)

As we head down to our front desk, let’s take a look through our hallways, or, our routers.

![Hotel MVC_ Into the Model-View-Controller (17)](https://user-images.githubusercontent.com/119631464/235601927-f76a476d-0e72-4c86-9709-90292a2bc652.svg)

In an MVC application, Routers are responsible for directing incoming requests to the appropriate Controller and Action. Routers are like the hallways in our hotel - they connect the different parts of the hotel (or the application) and provide a way for guests (or users) to get to where they need to go. 

Just like how our hallways have signs and arrows pointing the way, Routers have routes and parameters that guide the flow of traffic.

![Hotel MVC_ Into the Model-View-Controller (5)](https://user-images.githubusercontent.com/119631464/235601020-b2cebf67-7705-4d66-9e02-f6c13dd4e9da.svg)

Ahh yes, here is the Front Desk. Let’s get them checked in. 

![Hotel MVC_ Into the Model-View-Controller (6)](https://user-images.githubusercontent.com/119631464/235601047-3fd4f92f-7170-4cd1-8183-8312747afeef.svg)

The Controller in an MVC application is like the front desk in our hotel. It's where all the action happens - from checking in guests to answering their questions and coordinating their requests. 

The controller in the MVC architecture manages the flow of data and acts as an intermediary between the model and the view. It processes the user's requests and updates the model or the view accordingly. 
The Controller is like the conductor of an orchestra, making sure that all the different parts of the hotel (or the application) are working together in harmony.

![Hotel MVC_ Into the Model-View-Controller (7)](https://user-images.githubusercontent.com/119631464/235601108-1d200f01-49f8-43eb-8220-cde4180bd642.svg)

We’re going to pop behind the desk for a moment- It’s important for you to understand a bit how things work ‘behind the scenes’. 
You’ll be shadowing one of our Model Employees, Leon. 

![Hotel MVC_ Into the Model-View-Controller (8)](https://user-images.githubusercontent.com/119631464/235601121-df403b6c-9e43-4a4d-8eb6-722f34829c53.svg)

The Model in an MVC application is like the hotel staff in our hotel (our Model employee if you will). They're the ones who interact with the hotel's ledger (or database) to make sure everything is running smoothly. 


Our Model employees interact with the database or other data sources to persist and retrieve information. This includes tasks such as querying the database, creating or updating records, and performing validations on the data. They ensure that data is organized and accessible in a meaningful way for the application's (Hotel’s) functionality. They also provide mechanisms for notifying other components of the application about changes to the data. This can be achieved through events, callbacks, or observers, allowing other parts of the system, such as Views or Controllers, to react and update accordingly when the underlying data changes.

A Model Employee always checks to make sure that everything is accounted for and in its proper place. 

![Hotel MVC_ Into the Model-View-Controller (9)](https://user-images.githubusercontent.com/119631464/235601136-d706d625-ab51-4824-97d1-32f49e4b7134.svg)

Leon: *Alright, while you’re here, let’s take a look at the hotel ledger or, our Database. Not only will this hold all of the guest information but it also holds information for each room (or view)!* 

![Hotel MVC_ Into the Model-View-Controller (10)](https://user-images.githubusercontent.com/119631464/235601153-2133af31-65a8-4570-92f0-ca19f79e95ba.svg)

Leon: *In a database-driven application, the database is like the hotel's ledger. It's where we keep track of all the guests, their reservations, and even what specific ‘view’ they asked for!  
It is the key component that stores and manages the application's data.*

*The database provides a structured storage mechanism for persistent data, enforces data integrity by applying rules and constraints on the stored data and provides mechanisms to query and manipulate the stored data. It supports structured query languages (SQL) for relational databases or query languages specific to the database type (e.g., MongoDB Query Language for MongoDB). These languages allow developers to retrieve, insert, update, and delete data based on specific criteria and conditions. Handle large amounts of data and support high-performance access. Techniques like indexing, caching, and optimization are employed to enhance query performance and ensure efficient data retrieval. Databases incorporate security measures to protect sensitive data. This includes user authentication, authorization, encryption of data at rest or in transit, and other security features.*

*It's hotel's brain, keeping track of everything that's happening and making sure everything adds up at the end of the day.*

![Hotel MVC_ Into the Model-View-Controller (11)](https://user-images.githubusercontent.com/119631464/235601164-444f7814-6e0c-436f-929d-83d5f5d52d3b.svg)

Leon: *Before we step away, let’s give a good “MVC Hotel” hello to our Hotel Manager, Mx. Mongoose! Mx. Mongoose is my boss and we work very closely with each other!*

![Hotel MVC_ Into the Model-View-Controller (12)](https://user-images.githubusercontent.com/119631464/235601207-27156a25-4c4d-4194-909b-d949e3a919dc.svg)

Leon: *In a database-driven application, we may use an Object-Document Mapper (ODM) like Mongoose to help manage the data in the Model.* 

*Mongoose enhances the developer experience when working with MongoDB by providing an intuitive API, schema definition, validation, middleware support, and query-building capabilities. It simplifies the interaction with MongoDB, promotes code organization, and offers powerful features to streamline the development process.*

*Our Hotel Manager, Mx. Mongoose helps translate the hotel ledger (or database) into a format that's easier for the other hotel staff (or Models) to work with. They provide context, manage the details, and take care of the grunt work so the staff can focus on providing the best service possible to our guests.* 

**hotel manager, mx. Mongoose growls**

*Let’s not bother them too much.* 

![Hotel MVC_ Into the Model-View-Controller (13)](https://user-images.githubusercontent.com/119631464/235601234-b05330d4-c721-419a-aa59-3d6c81b0c084.svg)

Thank you, Leon! I will take over from here. 

Please follow me back through our models and our controllers to get to our final stop on our tour… our Views! 

*Ehem- Excuse me front desk (controllers), can you check to see our Ledger (Database) to see what rooms are available to view?* 
…
*Great, thank you.*

![Hotel MVC_ Into the Model-View-Controller (14)](https://user-images.githubusercontent.com/119631464/235601256-354b64b2-2eb5-450f-827b-cbc19ef4c522.svg)

**ding**

![Hotel MVC_ Into the Model-View-Controller (15)](https://user-images.githubusercontent.com/119631464/235601270-1302017d-d662-4854-b31b-6a821184e48e.svg)

WOW! What a view! 

The View in an MVC application is like the guest rooms in our hotel. Views serve as the bridge between the Model and the user, presenting the data in a visually appealing and interactive way. They're where the guests (or users) stay and get to enjoy all the amenities, like a comfy bed, fluffy pillows, and maybe even a minibar if they're feeling fancy. 

The View is responsible for making sure everything looks and feels great for the users and  ensure that the UI is visually appealing, consistent, and aligned with the application's design principles. They transform the raw data received from the Model into a format that can be easily understood and interpreted by the user. Views often utilize template engines or component-based frameworks to dynamically generate the UI based on the data. Engines like EJS, Handlebars, or JSX with React allow for the reusability of UI elements, separation of concerns, and easier management of UI components. 

When the Model (employee) is modified or updated (or re-trained), the Controller (front desk) notifies the View (our rooms division), triggering a refresh or re-rendering (or redesigning) of the relevant UI components (room layout). This ensures that the user always sees the latest data and reflects the current state of the application (or current layout of our room). 

By separating the presentation concerns from the underlying logic, Views contribute to a more modular, maintainable, and scalable application architecture.

![Hotel MVC_ Into the Model-View-Controller (16)](https://user-images.githubusercontent.com/119631464/235601294-322af63d-3c8d-490d-a306-fe3711dd0276.svg)


In conclusion, the Model-View-Controller (MVC) architecture provides a powerful framework for developing robust and maintainable applications. By separating the concerns of data management, user interface presentation, and application flow, MVC promotes code organization, reusability, and scalability. 

Understanding the roles of the Model, View, and Controller, along with the additional components such as Mongoose, routers, middleware, and databases, empowers developers to build efficient, modular, and user-friendly applications. 

Embrace the MVC principles and leverage these analogies to architect your applications with confidence!

![Hotel MVC_ Into the Model-View-Controller (1)](https://user-images.githubusercontent.com/119631464/235601369-b029cbf7-df96-44ff-bfc7-60ca92fd0d27.svg)







