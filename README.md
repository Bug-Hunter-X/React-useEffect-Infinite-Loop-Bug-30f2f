# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook and its dependency array.  The bug causes an infinite loop due to an incorrect dependency array in the `useEffect` function. 

## Description
The `useEffect` hook is used to perform side effects in functional components. However, omitting or incorrectly defining the dependency array can lead to unexpected behavior. In this example, the state `count` is updated within the `useEffect` but is not included in the dependency array, creating an infinite re-render loop. 

## Solution
The solution involves correctly defining the dependency array in the `useEffect` function. By including the `count` state in the dependency array, the effect will only run when the `count` value changes.