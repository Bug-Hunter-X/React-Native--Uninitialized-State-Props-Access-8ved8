# React Native: Uninitialized State/Props Access

This repository demonstrates a common error in React Native: attempting to access a state variable or prop before it's been initialized.  This frequently results in unexpected behavior or crashes.

The `Bug.js` file shows the problematic code. The `BugSolution.js` file illustrates a couple of ways to fix the issue.

**Problem:** The component tries to render using `this.state.data` even before it's fetched from an API call. This results in an error, because `this.state.data` is `undefined` during the initial render.

**Solutions:**
* **Conditional Rendering:** Only render the component's data-dependent elements after the state is populated.
* **Asynchronous Data Handling:** Efficiently handle asynchronous data loading to prevent premature rendering.

This example focuses on these common scenarios.