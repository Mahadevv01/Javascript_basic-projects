# JavaScript Concepts and Features Explanation

## **Features of the Project**
1. **Dynamic UI Updates**  
   - The project uses JavaScript to manipulate the DOM dynamically.
   - Tasks can be added and removed in real-time without refreshing the page.

2. **Event Handling**  
   - The `addTaskBtn` button listens for click events to add tasks.
   - Each task has a delete button that listens for a click event to remove it.

3. **Separation of Concerns**  
   - HTML for structure, CSS for styling, and JavaScript for functionality.
   - Encourages maintainable and scalable code.

4. **Interactive User Experience**  
   - Provides instant feedback when tasks are added or removed.
   

---

## **JavaScript Concepts**

### **1. Callback Functions**
- **Definition**:  
  A function passed as an argument to another function to be executed later.
  
- **Use Case**:  
  Useful for asynchronous operations like handling events or making API calls.

- **Example**:
  ```javascript
  function fetchData(callback) {
      setTimeout(() => {
          console.log("Data fetched");
          callback();
      }, 1000);
  }

  fetchData(() => {
      console.log("Callback executed!");
  });
