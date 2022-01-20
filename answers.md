- In action creators, like `getFilmFromAPI`, we use a "regular expression" ---
  what is that regular expression, and what is its purpose?
  /\d+/ , matches pattern for a series of digits
  
- We're persisting the Redux store, so if you re-visit the app, it will remember
  the topics you've visited. Where is this stored? How is this done?
  This is done with the persistgate component in index.js 
  
- What does `combineReducers` do? Why are we using it? 
  The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

- How does the "Reset to Fresh Exploration" feature work?
  clears state data from the store

- Why are `FilmList.js`, `PlanetList.js`, and 
  `PersonList.js` all simple components that use an `ItemList`?
  Why is this a good design?
  You want your components to be as simple as possible, and reduce rendundancy

- In the `HomePage` component we use the `useSelector` hook to save only a single fact---
  whether the first film is loaded, We could instead have selected all the
  films, and had the check for whether the first film is loaded in our
  `render` function. Why is this worse? What would the performance implications
  be?
  checking the data before he render would be faster than rendering and then checking the data
  
- What good ideas for designing and organizing React apps have you learned from
  studying this code?
  got a slightly better understanding of redux and 
  
- Which Star Wars character would make the best React developer, and why?
  Yoda, easily
  
