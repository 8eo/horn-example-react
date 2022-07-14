# Horn examples

Horn is a super-flexible communication platform that you can use to build
your own applications and interfaces. 

We're building a JavaScript API library, that should work in every web-based environment. 
But you can also use it in NodeJS itself when you don't want to have streaming part of our API (i.e. all
you want to do is to use REST API).

This repository contains examples of how our JavaScript API can be used to start building
applications in various frameworks like React or AngularJS.

Our JS API is written as an ES Module and published on our own NPM repo.

All examples requires you to have our `@horn/api` package installed:

```bash
npm install --registry=https://npm.horn.co --save @horn/api 
```

> :warning: These examples assumes you already have created a guest-allowed channel and you
> know it's UUID. You can create channels using REST API (after getting an API Token from the Horn team)
> or via the Horn Management Console.

We'll do a few things in the example:
1. Figure out client ID based on our channel ID
2. Create a random guest user
3. Configure JS API to connect to our channel with that user
4. We'll accept an invitation to move from the Lobby to the channel
5. After 2 seconds we'll try to share the camera

> :bulb: To see if this really works, you can go to the channel, login, and wait
for that new guest user to join.

Learn more for a specific framework:

* [React](./react/)
* [Angular](./angular/)
