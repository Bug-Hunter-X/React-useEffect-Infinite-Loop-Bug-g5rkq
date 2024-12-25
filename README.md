# React useEffect Infinite Loop Bug
This repository demonstrates a common React bug involving the `useEffect` hook and its dependency array. The bug causes an infinite loop due to improper usage of the dependency array. 

## Bug Description
The `useEffect` hook is designed to perform side effects after a component renders.  However, if the dependency array is missing or incorrect, the effect can run repeatedly, creating an infinite rendering loop.

## Bug Reproduction
1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console output and the component's behavior.  You'll see continuous console logs, indicating the component is rendering indefinitely.

## Solution
The solution lies in correctly specifying the dependency array for the `useEffect` hook.  By including the `count` variable in the dependency array, the effect only runs when `count` changes. 
