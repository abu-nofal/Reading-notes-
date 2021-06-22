## React and Forms 

1. What is a ‘Controlled Component’?

- it’s convenient to have a JavaScript function that handles the submission of the form and has access to the data that the user entered into the form 

- An input form element whose value is controlled by React 

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.


- we should update the state with their responses as soon as they enter them (to be more dynamic and to display the state for them after submit , the displayed value will update as the user types)




3. How do we target what the user is entering if we have an event handler on an input field?

- with even.target.value of the user input 

- we add attribute  value for the input elemnt and then target with event



## The Conditional (Ternary) Operator Explained

1. Why would we use a ternary operator?

- its shorter thin the if statement 
- redues time 
- more cleanr thin if statement  

2. Rewrite the following statement using a ternary statement:

>  ` if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }`

  > the ans =====> 
  ` x===y ? (console.log(true)) : (console.log(false)) `



[React and Forms](https://reactjs.org/docs/forms.html),

[The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)