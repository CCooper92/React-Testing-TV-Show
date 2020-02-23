# React Testing TV Show

## Advanced Web Applications

## Testing React

## Objectives

- use mocks in unit tests
- test asynchronous API calls that are made in a component
- test React components as the props change

## Introduction

As a developer, you will be asked to write tests for the feature you are building, and even sometimes on components and features other developers have built. This project will mimic a situation where you are asked to test someone else's code.

Get the project fired up and start using it as a user would. Try to go through the user sequences for this feature that you think users would go through. Once you have those in mind, you will have an idea of what to test in your application.

## Instructions and/or completion requirements

Your challenge for this module: write tests for both the `App.js` component and the `Episodesjs` component. Take note of where the state is being managed, where the async call is, and where different data peices are being rendered. Understanding all of this will be important so you know how to test each component.

**Moving the async call**

The async call being inside the component makes it hard to test the asynchronous nature of the component. Let's move the async function into an `/api` directory so we can easily mock that function and make the async tests easier.

1. Create a directory called `/api` in the `src` directory
1. Create a file inside `/api` called `fetchShow.js`
1. Move `fetchShow` into that new file and export it (fetchShow is in the `useEffect`)
  - Note that you need `axios` in this file
1. Import `fetchShow` into `App.js` so you can make your async call from your `useEffect` hook.

## Stretch goals

- There is an utility function in this project that contains an isolated pure function. Look up how to do `unit tests` with Jest and test that function.

- Look up the `TVMaze` API. Add a dropdown with the titles of some other popular shows. Add the user sequence of choosing a different show to fetch data for different shows.

- Add React Router, and add the functionality to click an episode and navigate to an episode page.
