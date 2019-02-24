# **Exercises**
## **Submit answers to the following questions:**

#### **1. In your own words, explain single-page applications and progressive web apps.**

Single Page Web Apps (SPA) are apps that literally only have one page. A SPA is super easy to display if compared to traditional server side rendered applications. It's really just one index.html file with a CSS Bundle and a JS Bundle. This type of deployment scales very well. 

On an SPA after the initial page load no more html gets sent over the network. Only data gets requested the server or sent to the server.

Examples of SPAs are 

www.google.com
www.gmail.com
google.maps.com

Progressive Web Apps (PWAS) are web applications that are regular web pages or websites but can appear to the user like traditional applications or native mobile applications. The applications type attempts to combine features offerred by most modern browsers with the benefits of a mobile experience. Currently Google, Microsoft, Mozilla, and other companies are working on a new, modern web application standard. PWAS are installable and live on the user's home screen, w/o the need for an app store. PWAs could be the next big thing for the mobile web. They can act like an android or ios app but you won't need to have an android developer or ios developer to build and maintain it. You will only need one, a web developer.




#### **2. Either from your research or by inspecting popular sites you frequent (using the Chrome DevTools), give some real-world examples of applications built with React and Angular.**

###Websites built with React - A Javascript library for building user interfaces.

https://www.airbnb.com/ Airbnb

https://www.atlassian.com/ Atlassian

https://www.facebook.com/ Facebook

https://www.paypal.com/us/home Paypal

https://imgur.com/ Imgur

https://flipboard.com/ Flipboard

https://www.dropbox.com/ Dropbox

https://www.bbc.com/ BBC


###Websites built with Angular.js

https://www.theguardian.com/us The Guardian

https://www.paypal.com/us/home Paypal

https://www.netflix.com/ Netflix

https://www.youtube.com/ Youtube

https://www.jetblue.com/ JetBlue

https://weather.com/ The Weather Channel

https://www.istockphoto.com/ iStock by Getty Images




#### **3. Write a summary of the benefits of React vs. Angular.**

React JS is a library instead of a framework. A library is a collection of prewritten code consisting of common tasks that simplify development.  The developers code is in charge when using React and uses a library to retrieve specific functions from the collection. Frameworks can be heavy handed and can limit you to doing tasks only one way whereas libraries are a tool that can be used to solve a problem ... you can use different tools in React to solve your problem different ways. In React you have much more control vs in Angular where Angular is dictating how things get done. React brought about coponent-based and unidirectional architectures for managing application state, including tools in the React ecosystem such as Flux, Redux, and RxJS. 

Benefits of Angular -

It is supported by Google. New changes before they are rolled out must pass through testing of Google's own 600 apps using Angular JS to insure they are not introducing new bugs. 

Per my Mentor React is far and away the most popular choice and many more developer jobs are looking for React experience vs Angular experience. That said some very large projects are already using Angular and that in itself would be very costly if they decided to change and use React so many larger companies are sticking with Angular because the cost to change is too much to justify the change. 

Angular JS is very popular among the banking industry. 

Angular is great for building single-page applications (SPAs). 

Angular which is a framework provides the basic structure of an application. A framework supplies the skeleton of a project which helps reduce the need for hard coding. The overall framework is based on components and services that you can think of as Lego blocks. All components and services start out the same way. For example, all Angular components do the following:

Import required ES2015 modules
Define a @Component decorator (metadata)
Place code in a component class

Angular provides a CLI tool that can be used to create initial projects, add different features into an application (components, services, etc.), run tests, perform builds, lint code, and more. This provides a great foundation for teams to build on to drive consistency across team members and even across multiple teams in an enterprise.

Angular has great consistency.  Consistency brings productivity into the picture as well. Developers don’t have to worry as much about if they’re doing it the “right way”. Components and services look the same overall, reusable application code is put in service classes, ES6/ES2015 modules organize related functionality and allow code to be self-contained and self-responsible, data is passed into components using input properties and can be passed out using output properties, etc.

With greater consistency, you get the added benefit of productivity. When you learn how to write one component you can write another following the same general guidelines and code structure. Once you learn how to create a service class it’s easy to create another one. It’s like a broken record consistently spinning round and round that feels like many other frameworks you may have used in the past. Combine all of this with the Angular CLI, code snippets that the team creates (or use mine if you use VS Code) and you’re consistent and productive.




