**Array Notes (Pt 2)**
[Also here](https://docs.google.com/document/d/1mzlV_QWwNgBnqEwoCjr57BNzGOdpTOduEf4wDik9hmo/edit?usp=sharing)

View Site here

- Variables declared with let can be reassigned.
- Elements in an array declared with `const` remain mutable:
    ```javascript
    let condiments = ['ketchup', 'mustard', 'relish'];
    condiments[0] = 'mayo';
    console.log(condiments); // Output: ['mayo', 'mustard', 'relish']

    const utensils = ['fork', 'spoon', 'knife'];
    utensils[2] = 'spork';
    console.log(utensils); // Output: ['fork', 'spoon', 'spork']
    ```
- One of an array’s built-in properties is length
- returns the number of items in the array
- **.push()**
- These methods are specifically called on arrays to make common tasks, like adding and removing elements, more straightforward.
We access the push method by using dot notation
- `.push()` can take a single argument or multiple arguments separated by commas.
```javascript
utensils.push('spork', 'napkin');
console.log(utensils); // Output: ['fork', 'spoon', 'spork', 'napkin']
```
- **pop()**
- removes the last item of an array
- does not take any arguments
- method that mutates the initial array
- returns the value of the last element

```javascript
const chores = ['do laundry', 'clean the floor'];
chores.push('clean the bathroom', 'take out the trash');
const removed = chores.pop();
console.log(chores); // Output: ['do laundry', 'clean the floor', 'clean the bathroom']
console.log(removed); // Output: 'take out the trash'
```
