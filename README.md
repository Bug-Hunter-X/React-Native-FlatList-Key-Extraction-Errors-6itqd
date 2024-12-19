# React Native FlatList Key Extraction Errors

This repository demonstrates a common error in React Native's `FlatList` component: improper or missing `keyExtractor` functions.  Using the index as the key, or omitting the `keyExtractor` altogether, can lead to significant performance problems and rendering bugs.  The provided code examples illustrate the incorrect usage and offer a solution using a unique identifier for each item.

## Bug

The `FlatListBug.js` file showcases the erroneous implementation.  It demonstrates how using the index as a key or completely omitting `keyExtractor` leads to unexpected behavior during data updates.

## Solution

The `FlatListBugSolution.js` file presents the correct approach, using a unique identifier from each item as the key.  This ensures that `FlatList` can efficiently update the list and avoids issues caused by index-based keys.

## Usage

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npx react-native run-android` or `npx react-native run-ios` to test the code.