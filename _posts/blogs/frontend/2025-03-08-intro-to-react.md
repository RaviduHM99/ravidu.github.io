---
title: 2. Introduction to React.js
description: >-
  Learn the fundamentals of React.js, a powerful JavaScript library for building user interfaces. This guide covers components, JSX, and state management for beginners.
author: ravidu
date: 2025-03-08 10:00:00 -0500
categories: [Blogging, Frontend]
tags: [react javascript]
pin: false
blog: true
image:
  path: /assets/img/blogs/frontend/react_logo.png
  lqip: data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA4MDAgNDUwIj48ZmlsdGVyIGlkPSJiIj48ZmVHYXVzc2lhbkJsdXIgc3RkRGV2aWF0aW9uPSIxMiIgLz48L2ZpbHRlcj48cGF0aCBmaWxsPSIjMjcyYzQ1IiBkPSJNMCAwaDgwMHY0NTBIMHoiLz48ZyBmaWx0ZXI9InVybCgjYikiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNiAxLjYpIHNjYWxlKDMuMTI1KSIgZmlsbC1vcGFjaXR5PSIuNSI+PGVsbGlwc2UgZmlsbD0iIzYxZGFmYiIgcng9IjEiIHJ5PSIxIiB0cmFuc2Zvcm09Im1hdHJpeCgtMTkuNzM4NzYgLTI2Ljg3MTA2IDc2LjkzMjc1IC01Ni41MTI3MyAyNDcuOCAxMDguMikiLz48ZWxsaXBzZSBjeD0iNjciIGN5PSIyNDEiIHJ4PSIyNTUiIHJ5PSI0MCIvPjxwYXRoIGQ9Ik03NiA2Nkw4IDgxbDMwIDE4eiIvPjxlbGxpcHNlIHJ4PSIxIiByeT0iMSIgdHJhbnNmb3JtPSJtYXRyaXgoLTkuMDE3NzQgLTIzLjQ1NzEzIDI3LjQwMDc1IC0xMC41MzM4IDM1LjYgNzQpIi8+PC9nPjwvc3ZnPg==
  alt: React Logo
---

## Understanding React Components

React is built on the concept of reusable components. Each component is a JavaScript function or class that returns JSX (JavaScript XML), which describes what the UI should look like.

### Basic Component Structure

```javascript
function Welcome() {
  return <h1>Hello, React!</h1>;
}
```

This is the simplest form of a React component. The component returns JSX, which looks like HTML but is actually JavaScript.

## Working with Props

Props are how you pass data from parent components to child components. They work similarly to function parameters.

### Example with Props

```javascript
function Greeting(props) {
  return <h1>Hello, {props.name}!</h1>;
}
```

## Next Steps

In the following tutorials, we'll dive deeper into hooks, state management, and building more complex applications.
