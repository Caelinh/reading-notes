# Loops #

## Loops ##
Loops are a way to do something repeatedly. do this then that. They repeat an action a certain amount of times.  
Format is  
`for ([initialExpression]; [conditionExpression]; [incrementExpression])    
statement`  
Example:
```function howMany(selectObject) {
  let numberSelected = 0;
  for (let i = 0; i < selectObject.options.length; i++) {
    if (selectObject.options[i].selected) {
      numberSelected++;
    }
  }
  return numberSelected;
}

const btn = document.getElementById('btn');

btn.addEventListener('click', () => {
  const musicTypes = document.selectForm.musicTypes;
  console.log(`You have selected ${howMany(musicTypes)} option(s).`);
});
```
## While ##
executes the statement as long as condition is true.
```
While(condition)
Statement
```

```
let n = 0;
let x = 0;
while (n < 3) {
  n++;
  x += n;
}
```
*With each iteration, the loop increments n and adds that value to x*
if condition becomes false statement  
inside of loop will stop executive and control does to the next statement outside of loop.  
