# A little about me

My name is Nima Soufiani, I know, kind of a rare name and a nightmare to spell for others. I'm a highly driven developer/engineer with a passion for AWS infrastructure, AWS Architecture and serverless development. My ability to learn and absorb information has led met to pursue and develop my skills within the AWS space. I have recently gained qualification as a AWS Certified Solutions architect - associate and have taken on responsibilities for managing and advising on cloud infrastructure within Ripple Energy. I also champion and develop serverless architectures for the different services at Ripple Energy to drive down costs, increase scalability and resiliency as well as improving on security for our cloud infrastructure.

## Table of content

- [My past](#my-past)
- [What I'm doing now](#what-i'm-doing-now)
- [Skills with Repo reference](#skills-with-repo-reference)
- [Education](#education)
- [Experience](#experience)
- [Blog](#blog)
- [Certifications](#certifications)
- [Hobbies and other interesting things](#hobbies-and-other-interesting-things)

## Projects

| <p align="center">Project</p>                             | <p align="center">Description</p>                                                                                                                                                                                                                                                   | <p align="center">Tech stack</p>                                                                                              | <p align="center">Link</p>                                                                                                                         |
| :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p align="center">AWS Serverless access keys rotation</p> | <p align="center">It is good security practice to rotate your AWS Access keys. Why not automate this process and make use of some of the awesome services AWS has to offer?</p>                                                                                                     | <p align="center">SAM, Lambda, SQS, SES, SNS, DynamoDB, Cloudwatch Scheduled events, Secrets Manager, IAM Resource policy</p> | <a href="https://github.com/Nimzyow/aws-serverless-access-keys-rotation" rel="some text"><img src="https://github.com/favicon.ico" width="48"></a> |
| <p align="center">DateSpot React-Native</p>               | <p align="center">The React-Native version of DateSpot. I wanted to prove that I could pick up a new testing framework, react-native-testing-library and TDD DateSpot with React Native. Not only did I manage that but I got the app working on a phone which was pretty cool!</p> | <p align="center">React Native, Redux, Jest, react-native-testing-library</p>                                                 | <a href="https://github.com/Nimzyow/datespot-reactnative" rel="some text"><img src="https://github.com/favicon.ico" width="48"></a>                |
| Thermostat                                                | This was a passion project inspired by a Makers Academy Thermostat challenge. I decided to challenge myself by completing this challenge with Node.js and Express.js for the backend and React for the front end.                                                                   | React, Node, Express, Jest and Enzyme, Cypress                                                                                | <a href="https://github.com/Nimzyow/thermostat_node_react" rel="some text"><img src="https://github.com/favicon.ico" width="48"></a>               |
| <p align="center">Client Database Management</p>          | <p align="center">A full stack React application made to manage clients and tasks for clients. Made to save time and to efficiently search for clients based on name, email and project description.</p>                                                                            | <p align="center">React, Node, Express, Context, Materialize</p>                                                              | <a href="https://github.com/Nimzyow/client_database_management" rel="some text"><img src="https://github.com/favicon.ico" width="48"></a>          |

## My past

During one of my many travels to Japan, I came across as a software developer working in Silicon Valley in 2018. After expressing my interest in software development and showing him my attempt at creating a Scuba Diving application for mobile with Unity and C# (I didn't know any better at the time), he showed me React Native and briefly gave me a rundown of what I needed to learn if I wanted a career as a Software Engineer.

After that fateful day, I very quickly became hooked on coding, like it was my true calling. I was endlessly sitting in cafes, going through Udemy courses like some prime time Netflix show and endlessly creating, testing and experimenting with different technologies.

Soon after, I finished a 16 week intensive bootcamp at Makers Academy to help fill in any knowledge gaps I have. They follow a TDD approach and they believe very strongly in the idea of collobaration through teamwork and pair programming.

## What I'm doing now

Fast forward to now I'm proud to have now become a highly capable Full Stack developer with a passion for AWS serverless computing. I now regularly spend my time spinning up lambda functions and creating queues doing all sorts of compute triggered by all sorts of events.

Working for a fast moving startup like Ripple Energy for 2 years as a Full Stack Software Engineer, I have had the unique opportunity to play a big part in the development process and modernise different areas of the codebase from frontend, backend to DevOps including utilisation of AWS services such as EKS, S3, EC2, Lambda, SQS, SNS, IAM and more.

I spear headed and implemented Ripple Energy’s first and subsequent serverless microservices solutions by writing infrastructure as code using SAM template files. This has enabled us to easily create scalable and secure cloud resources while following the principles of least privilege when creating IAM policies, all while saving on costs.

I'm a qualified AWS Certified Solutions Architect - associate and am actively working towards a qualification for AWS Certified Developer - associate. The more I delve into the Serverless world the more I geek out over the fact that I can create an ecosystem where a developer only has to worry about code and not infrastructure. I'm constantly fascinated by how I can make different services work together to create a cost effective, highly scalable and durable infrastructure for web applications that live in the cloud. My hope is to be working more in this field in the future.

## Skills with Repo reference

### AWS Serverless access keys rotation

After passing the AWS Certified Solutions Architect - associate exam, I felt that I wanted to use my skills in a meaningful way, straight away. After making an assessment on security regarding our cloud infrastructure, I felt it was necessary to automate our AWS Access keys to follow security best practices.

I decided this would be a fantastic first dip into the serverless world and I decided to create: [AWS Serverless access keys rotation](https://github.com/Nimzyow/aws-serverless-access-keys-rotation).

There were many services that were of interest to me such as SQS, SNS, SES, Lambda etc.. and I was eager to experiment with these services by writing a SAM template file. But first, I had to diagram the architecture out, which I have included in the repo. After that, it was onto writing SAM template files.

This was a great lesson in writing infrastructure as code. I had a lot of fun creating resources for lambda functions, SQS queues, SNS topics, DynamoDB table, SES and a Cloudwatch Schedule event. I also made extensive use of the @aws-sdk to write my lambda functions.

I also developed the Github Actions flow with the help of the `sam pipeline` to automate safe deployments from my staging to production account.

This project was also unit tested using jest unit testing and the lambda functions were written in TypeScript to increase resiliency within the lambda functions.

Plans for the future is to convert this project into step functions as I feel step functions are a more appropriate solution to the many Lambda + SQS queues that are currently here. But one learns from repetition which is why it was architected the way it was.

Overall, this was a great first taste into the serverless world and this project really got me eager to do more projects within the AWS ecosystem.

### Node, Express and React:

I created a Full Stack MERN application based on the final project I was a part of at Makers Academy. [DateSpot](https://github.com/Nimzyow/datespot). The entire application was TDD'd from beginning to end. The original projects front end state management was handled by React's Context API. I decided to switch state management to Redux through TDD. This was a great challenge that enabled me to learn and understand Redux further. The TDD of the backend was especially insightful and went through multiple reworks with the aim of it being more readable. Testing was done in Jest and Enzyme, Supertest, Mocha and Chai. I alaos switched the original projectsdatabase from SQL based to NoSQL, MongoDB.

During Makers we were asked to make a thermostat web application with Jquery and testing in Jasmine. I decided to take that idea and use Node.js, Express.js and SQlite for the backend and use React for the front. The TDD approach was taken using Jest and Enzyme for unit testing and Cypress for feature testing. [thermostat_node_react](https://github.com/Nimzyow/thermostat_node_react)

My first attempt at a full stack MERN application can be seen in my repo: [client_database_management](https://github.com/Nimzyow/client_database_management). I used hooks for better readability and context for state management. I also used Node.js, Express.js and MongoDB for the backend.

### Ruby on Rails and React

As part of our final project in Makers, we were tasked with creating an application to present to a live audience in just over a week. This project, called DateSpot, was challenging not just from a technical perspective, but from the perspective of working in a team enviornment and getting the best out of everyone in the team. Overall, we were very successful and created an awesome application with the backend done on Ruby on Rails, set up as an API and the frontend being done entirely in React with Reacts Context API for state management. The link to the repo: [DateSpot](https://github.com/rafahg/travel-final-project). The presentation for this project can be found on the following link just after the 3 minute mark: [Presentation](https://www.facebook.com/watch/live/?v=1854532374684301&ref=watch_permalink)

### React Native:

After DateSpot I decided to create the React Native version so that I could try out a new testing framework. Basically, I wanted to see this run natively on my phone! [DateSpot](https://github.com/Nimzyow/datespot). The entire application was TDD'd from beginning to end. Since I was TDD'ing with react-native-testing-library, it required a lot of playing around but I found it very intuitive and brilliant, in fact. Since the backend and front end of the application were decoupled when I created the React version, it was relatively straight forward to TDD this application.

My first attempt at making an Engineering application for iOS and Android can be seen in my repo "iEngineer". It was a great learning experience and taught me many things, particularly about the horrors of not keeping clean code. Again, I kept this repo there to remind myself how I started.

### Redux:

The repo [ITLogger](https://github.com/Nimzyow/ITLogger) is a ITLogger application created with Redux for state management. It was created to dimystify the whole process of Redux. [ReduxLearning](https://github.com/Nimzyow/ReduxLearning) is a simple repo created to internalize the basics of Redux.

## Education

### Makers Academy (February 2020 to May 2020)

- OOP, TDD, MVC, DDD
- Agile/XP
- Ruby, Rails, JavaScript, HTML, CSS, React
- RSpec, Jasmine, Cypress, Jest and Enzyme
- MongoDB, Sequelize, SQL, PostgreSQL, sqlite

### University of East London / College (2007 to 2011)

- BEng Civil Engineering
- 1st class
- Started the UEL Civil Engineering society

### University of East London / College (2011 to 2012)

- MSc Structural Engineering
- Merit

### Udemy courses completed

Complete React Native Bootcamp - Build 18 iOS & Android Apps
Credential ID UC-370G30HA

React Front to Back 2019
Credential ID UC-GPN7KGZL

Testing Ruby with RSpec: The Complete Guide
Credential ID UC-977106dc-164e-43e8-993a-98bfff3c3a3a

### Other courses completed

Advanced Open Water Diver - PADI

Digital underwater photographer - PADI

Enriched Air Diver - PADI

## Experience

### Ripple Energy (August 2020 - present)

_Full stack software engineer_

Currently working as a Full stack software engineer and making a difference in the clean energy sector through code. It is a dynamic working environment where we are encouraged to self learn and take charge of our code, the emphasis being clean, maintainable and readable code.

### Freelance (Feb 2020 to May 2020)

_Student_

Finished a highly intensive bootcamp after making a real commitment to becoming a software developer. The 16 week intensive course filled any knowledge gaps I had from my own self learning and has made me very confident as a software developer.

**Achievements include:**

✓ Learned and honed in the value of TDD. Consistent 95% or greater test coverage is maintained throughout any applications we develop.

✓ Successfully collaborating with peers with different backgrounds and
programming level, through pair programming, in an agile
environment.

✓ Strengthened my already greatest asset of self-learning to enable me
to learn any technology required within a short space of time.

✓ Created a cool application in a group of 5 people as part of our final project utilising everything we have learned throughout the bootcamp from agile processes to creating a working environment where everyone is allowed to have their say.

Languages, Frameworks and Tools: React, Hooks and Context API, Bootstrap, Jest and Enzyme, Cypress, Ruby on Rails, Active Record.

### Makers (August 2019 to Dec 2019)

_Full Stack Developer_

The firms handling of client information required modernising. I developed a full stack client database web application to help staff with client database management. Currently working on React Native version.

**Achievements include:**

✓ Staff can now create, read and update clients.

✓ Enabled functionality to drastically reduce search time for projects with associated clients

✓ Staff are now able to add tasks to each client to better visualise what tasks are left outstanding.

✓ Enabled authentication and encryption to ensure safety of client details.

Languages, Frameworks and Tools: React, Hooks and Context, JavaScript, Node.js, Express.js, MongoDB. Currently planning on the React Native version of the same application.

### Civil Engineers Ltd (August 2012 to December 2019)

_Structural Engineer_

Worked as part of a team on up to 12 commercial and residential projects a month ranging in Capex investment and asset value from £50k to £1m.

**Achievements include:**

✓ Self-learnt and changed the way we work entirely through adoption of new technologies to drastically increase productivity by 10-fold

✓ Taught staff the benefits of using the newer technologies introduced and guided them on how to efficiently use them.

✓ Time needed to complete each project was cut back, on average, from a week to only one day.

## Certifications

AWS Certified Solutions Architect - associate - Oct 2022

AWS Certified Developer - Associate - Currently studying for

## Hobbies and other interesting things

I absolutely adore Scuba Diving and if I ever go on vacation, some scuba diving has to be involved! It is a real passion of mine and I adore looking at the different marine life and learning about them. Ship wrecks are also awesome and they fascinate me to no end!

![scuba](https://github.com/Nimzyow/CV/raw/master/media/PA280059rr.JPG)

I can speak Japanese to a near fluent level and have many friends in Japan who I love talking to. I learnt Japanese bit by bit over a number of years and I became obsessed with improving myself. This led to me making life long friends who I love dearly.

![travel](https://github.com/Nimzyow/CV/raw/master/media/P1010822.jpg)

Travel is probably a typical hobby that everyone has to put on their list. However, it really is something I love to do as it allows me to experience different cultures and people and to learn things from them. I often come back with a new perspective in life and a new way of looking at things.

Photography and the art of photography is something that really inspires me. I have a website www.foreverintransit.com which showcases some of my photography. My instagram is more up to date though and you can see that in the website I just linked.

![street](https://github.com/Nimzyow/CV/raw/master/media/DSC03703.jpg)
