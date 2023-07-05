# Modern React Guide

This guide will give you everything necessary to begin learning react, and make your own projects

# Basics to know

- Javascript
    - variables (let, var, const)
    - functions 
    - ES6 (EcmaScript 6, this is just a convention or standard of JS) 
    - JavaScript Objects 
    - Arrays
    - For loops
        - For in
        - For of
    - maps
    - filters
    - DOM manipulation

- Basic CSS

- HTML

# Functional React

First React is divided into two forms, class components (legacy) and functional components(modern), the scope of the guide is just functional components.

## Hooks

React has special functions called hooks, this are functions premade and served using javascript, and nodejs behind, this "Hooks" facilitates the coder's life by a lot, and perform complex operations that benefit both the performance and development of the website.

### Basic Hooks

The following are ordered in complexity order, this is the commonly found order to learn them:

- useState 
    - performs component state management, the concept of "state" on it's own is very deep, so you must read about it.

- useEffect
    - performs a change on the frontend when something takes effect, e.g when you login, and the screen loads, it triggered an event, and "something took effect" this something could be an API call.

With these two hooks, you can create virtually any site, although it would lack performance optimizations,

### Intermediate Hooks

- useCallback
    - Gives performance speedup by caching on memory a repetitive function, e.g, an animation needs to perform a lot of matrix calculations, and it's repetitive, you could cache it, so the website wouldn't need to recalculate often.

- useMemo
    - Same concept of useCallback, but applies for whole components.

- useRef
    - Refs are used when data must be persisted between renders, this is similar to the concept of state, the key difference is the persistance, meanwhile the state disappears when it's re-rendered.

- useContext

    Let's say you have a lot of state variables, and nested components, you can reduce the complexity of the state management by using a Context, the context allows multiple components to acces to the same state, this reduces code, and gives better performance.

### Advanced Hooks

There's just a couple of hooks remaining, but the most important would be:

- useReducer

    A Reducer is a different way to treat state variables and functionality, again the concept of state  can be very complex, so much that libraries have been created to solve state management while optimizing the performance of the code and development time, so useReducer is React's response of not using a 3rd-party library.

    useReducer is used in a way that you can access an internal state on any component(similar to Context), make some changes, store it, even persist it(similar to Refs), pretty much the combination of other hooks. A common example is the following:

    You have an e-commerce app, under the checkout section, the user can modify the quantities of objects they're buying, by clicking some buttons, etc. So the user deletes a product (pops out of the list of products), then clicks a new section of the site (FAQ), later returns to the Cart Section, and all of this, without calling an API, just to get the items they want to buy, reducer allows this interaction.

    In summary Reducer can be complex, to describe, due to the nature an applications of it, of course it isn't mandatory to know how to use it, as you can always do another logic just by using raw useState, etc. or using external libraries.


# Libraries

React can benefit from libraries, and these varies on the usage, some useful libraries:

- Global State Management:
    - Redux Toolkit (the most popular, really useful)
    - ImmerJS (not that popular, and low level)
    - Zustand (popular, easier then redux)

- Forms

Forms are really repetitive tasks on front-end, and tedious sometimes for that these makes your life easier:
    
- React-Hook-Form (provides hooks, global state management for forms, amazingly powerful)
- Formik (older the the first own, pretty good for simple forms)

## Beyond WebSites

React is made to run on a webserver, but an extension was made, React is actually capable of running on any platform, one of these is mobile.

### Mobile Apps

You have React-Native, you basically can create an IOS/Android app, by using React-Native, JavaScript, CSS, etc, and you'll have an app on both platforms ready to be deployed, now react-native is in essence just React, but it needs a lot of advanced concepts of vanilla javascript and React Hooks, as you need to squeeze everything ot make the app as smooth as possible. But React-Native is a different story.




