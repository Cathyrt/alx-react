# 0x08. React Redux Reducer and Selector

In this module, we will look into the fundamental concepts of Redux reducers and selectors within a React application. Understanding how reducers and selectors work is essential for maintaining a predictable state management system and optimizing the performance of your application.

## Table of Contents

- [Purpose of a Reducer](#purpose-of-a-reducer)
- [Role of a Reducer](#role-of-a-reducer)
- [Keeping Reducers Pure](#keeping-reducers-pure)
- [Avoiding Mutations in Reducers](#avoiding-mutations-in-reducers)
- [Using Immutable Data](#using-immutable-data)
- [Utilizing Normalizr](#utilizing-normalizr)
- [Selectors: What and When](#selectors-what-and-when)

## Purpose of a Reducer

A reducer is a core concept in Redux, responsible for specifying how the application's state changes in response to actions. It's a pure function that takes the current state and an action, then returns a new state. Reducers help maintain a centralized and predictable state management system, making it easier to understand and debug application behavior.

## Role of a Reducer

Reducers play a crucial role in the Redux architecture by:

- Listening to dispatched actions.
- Determining how the state should change based on the action type and payload.
- Returning a new state object that reflects the changes.

## Keeping Reducers Pure

Reducers should remain as pure functions. This means they should not have any side effects and should always return the same output for the same input. Keeping reducers pure ensures predictable state changes and easier testing.

## Avoiding Mutations in Reducers

Mutating the state directly within a reducer can lead to unexpected behavior and make it challenging to track changes. Instead, always create new objects or arrays when making updates to the state. This maintains the immutability of the state and helps with debugging and tracking changes.

## Using Immutable Data

Immutable data ensures that the state remains unchanged once it's created. This is crucial for tracking changes and enabling features like time-travel debugging. Libraries like Immutable.js can be used to create and manage immutable data structures.

## Utilizing Normalizr

Normalizr is a library that simplifies the process of normalizing nested data structures. It helps in flattening complex data into a normalized form, which makes it easier to manage relationships and reduces redundancy in the state.

## Selectors: What and When

Selectors are functions that extract specific pieces of information from the Redux store. They provide an abstraction layer between the application and the state tree. Selectors help in encapsulating the structure of the state, making it easier to refactor the state shape without affecting the components that rely on it. They are especially useful when dealing with complex state structures or when optimizing performance by avoiding unnecessary re-renders.

Remember, understanding how to use reducers and selectors effectively is crucial for building scalable, maintainable, and performant Redux applications.

---
