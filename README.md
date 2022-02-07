<p align="center">
  <a href="https://rfcsapi.com/" target="blank"><img src="https://rfcsapi.com/assets/images/logo.png" width="320" alt="Boilerplate Plaftorm" /></a>
</p>

<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

## Features ✨

### Modules

1. [Boilerplate Backend Server](https://github.com/ialopezg/boilerplate.git). Core module. Will expose the Boilerplate Platform API for its Business Logic with public and private API endpoints. Will not be direct accesible by common users or apps only if business rules are applied. This application will be intended only for act as an intermediary to response all request coming from any application that is contained in Boilerplate Platform.
2. [Boilerplate Back Office](https://github.com/ialopezg/boilerplate.git) Administrator Office for Boilerplate Platform. All administrative task will be done accross this app. Supports web, desktop, and mobile environments.
3. [Boilerplate Client App](https://github.com/ialopezg/boilerplate.git). Intended to be used for common users that could donwload and install it into their devices. Its use will be regulated and normalized by the business logic and rules could be applied. Supports web, desktop, and mobile environments.
4. [Boilerplate Client Web](https://github.com/ialopezg/boilerplate.git). Main frontend of Boilerplate Platforms.
5. [Boilerplate Resource Assets](https://github.com/ialopezg/boilerplate.git). Contains all assets as images, animations, fonts, and all related content specific for the UI/UX.

### Technologies

![TypeScript](https://img.shields.io/badge/-TypeScript-000000?style=flat&logo=typescript)
![JavaScript](https://img.shields.io/badge/-JavaScript-000000?style=flat&logo=javascript)
![Java](https://img.shields.io/badge/-Java-000000?style=flat&logo=java)
![Flutter](https://img.shields.io/badge/-Flutter-000000?style=flat&logo=flutter)
![Dart](https://img.shields.io/badge/-Dart-000000?style=flat&logo=dart)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-000000?style=flat&logo=postgresql)

## Getting started ✨

```bash
# 1. Clone the repository
git clone https://github.com/ialopezg/boilerplate.git

# 2. Enter your newly-cloned folder
cd boilerplate

# 3. Update latest repository commits from origin
git submodule update --remote --merge

# 4. Sync modules
git submodule sync

# 5. Enter desire repository and follow the instructions inside the repository chosen.

# 6. Read the documentation linked for each module for more details.
```

## Documentation ✨

Each module project includes a `docs` folder with more details.

## Development Phases

This section describes the phases of development where we will have "Major" version releases. A product of this size is never built in one go, in fact, the separate components as shown above is not even built to completion in any phase. We've moved away from Waterfall a while back and the most successful software companies do incremental work / updates given we're almost the only field in engineering that can do that without any additional cost. We'll have multiple phases marked by specific functionality being in that phase which will give us a nice break down of what to work on in order to complete the development of this application.

The phases are all dependent on the architecture showed above, the parts with the most dependencies will most likely be built first so we can allow for multiple other parts to be worked on as well. Lets go over a basic high level view of some of the phases.

### Phase 0: Technical architecture overview and technology stack setup

This is the high level technical phase of the planning that was done above. We need to establish how we will be building these management services, how they will be deployed, how the source code will be managed and how we plan on extending functionality / deprecating older functionality. This is an important part since the services will be the major feature of the project. We are skilled at developing client applications, and stacked is our preferred architecture, with this planning we'll need to setup the backend in such a way that it's easy to unit test, easy to deploy, easy to manage, easy to update and easy to debug in the live production state.

This phase will be concluded when we have a detailed plan of the technical setup and technical architecture overview as well as the deployment and technology stack overview.

### Phase 1: Technical Internal overview and data storage structure

In this phase we want to go over all the functionality we're looking at adding into each project. This will illuminate how we have to build the inter communication methods as well as the models that we'll require to build all the functionality. We will walk through the most important processes required and do a highlevel step list of how the data will move from the client through our backend and back to the client. When this is complete is necessary identify key models and decides on which properties will be useful to have in the application.

A success for this phase will be a detailed breakdown of one of the key processes, which models will be in the application as well as the purpose they serve, their properties and in which parts of the system they will be used in. This will give us a decent framework to criticise in an engineering meeting to make sure we have no gaps in our system.

### Phase 2: Data population and development prep

In this phase we are still not writing code haha. Planning and structure is important for such a large system, and we're still going to miss things. Here we will use the models defined above and generate some fake data for use to use when we finally do start the development. This process will give us a first review of our database structure we defined above and will show any flaws that we might have made in terms of how to store everything. This will also be very helpful during the development to ensure that we have data to work it.

A success for this phase will be a database with enough information in it to allow us to display some basic product when we get to that point. 

### Phase 3: Customer App Setup and Authentication

Here we will create the mobile flutter project and setup firebase authentication. We will also make sure that when a user signs up we create them a profile on the database where we can manage all their information. This will be profile information for us to identify who we're communicating with.

A success for this phase will be a flutter app where we can sign in. A folder with a firebase project for user management that contains the cloud function to create a new user model entry in firestore when the user is created. A firebase app setup to allow for authentication.

### Phase 4: Which information do we show?

Usually in geolocation service it only shows devices that are between10 - 20 km radius. We need to build that system first before we can show devices to the user. For this we'll be using gmaps to get the users address and then use that locally to calculate which devices will be show.

## Support ✨

[Boilerplate Platform](https://github.com/ialopezg/boilerplate.git) is proprietary licensed project. It can grow thanks to the sponsors and support by the amazing backers.

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/ialopezg"><img src="https://avatars.githubusercontent.com/u/6828828?s=100&v=4" width="100px;" alt="Isidro A. López G."/><br /><sub><b>Isidro A. López G.</b></sub></a><br /><a href="https://github.com/ialopezg/boilerplate/issues?q=author%3Aialopezg" title="Bug reports">🐛</a></td>
  </tr>
</table>


## License

Copyright © 2022 - Boilerplate Platform. This source code is licensed under the Proprietary License found in the [LICENSE](LICENSE) file.

---

BOILERPLATE Platform - by [Isidro A. López G.](https://ialopezg.com/)
