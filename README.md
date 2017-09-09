# Bookkeeper Api

![Bookkeeper Api](https://media.giphy.com/media/l0IyeL8r9UhJI5LcA/giphy.gif)

Join or create a Shared flat with your roommates, track your common expenses. 

## Pre-reqs
- Install Docker 
- Install Docker-compose

## Getting started
- Clone the repository
```
git clone git@github.com:Edouardbozon/bookkeeper-api.git
```
- Jump in dir
```
cd <bookkeeper-api>
```
- First time, build and run containers
```
docker-compose up --build
```
- :rainbow: It works! navigate to [http://localhost:3000](http://localhost:3000)

- Next time, just run containers
```
docker-compose up
```

## Road map

There is a lot of things to do:

1. Switch the app in full api mode
2. Make a full crud for public shared flats routes and enhance domain logic
    - :white_check_mark: Add ability to do a request to join a shared flat
    - Add ability to modify a shared flat by an admin
    - Add query data validation to create a shared flat
    - :white_check_mark: Add user verification to create or join a shared flat (user can only be in 1 shared flat)
    - Add single shared flat route detail as "profile" page for people that are outside
    - Add tests
3. Add private shared flat functionnality (only navigable by the residents)
    - Add list common expenses route
    - Add ability to add common expense 
    - Add tests
4. [Further] Add geo search for shared flats to join them more easily
    - Maybe use Elasticsearch to provide geo-search ?
5. [Further] Add realtime shared flat expenses tracking
    - Maybe use socket.io ?

## Helpfull Links

- [NodeJS](https://nodejs.org/dist/latest-v8.x/docs/api/)
- [TypeScript cookbook](https://basarat.gitbooks.io/typescript/content/docs/getting-started.html)
- [Express/TypeScript starter](https://github.com/sahat/hackathon-starter.git)
