## Arrow Function

### Example 1
```javascript
const tasks = {
  tasks: [{
    text: 'Buy new shoes',
    completed: true
  }, {
    text: 'Clean keyboard',
    completed: false
  }, {
    text: 'Watch Umbrella Academy',
    completed: false
  }],
  getTasksToDo () {
    return this.tasks.filter((task) => task.completed === false)
  }
}

console.log(tasks.getTasksToDo())

/* Output:
[ { text: 'Clean keyboard', completed: false },
  { text: 'Watch Umbrella Academy', completed: false } ]
*/
```

### Example 2
```javascript
const event = {
  name: 'Birthday Party',
  guestList: ['Ge', 'Jane', 'Mai'],
  printGuestList: () => {
    console.log('Guest list for ' + this.name);

    this.guestList.forEach((guest) => {
      console.log(guest + 'is attending ' + this.name)
    })
  }
}

event.printGuestList()

/* Output:
Guest list for Birthday Party
Geis attending Birthday Party
Janeis attending Birthday Party
Maiis attending Birthday Party
*/
```