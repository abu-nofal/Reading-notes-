# Review, Research, and Discussion

1. **Describe (in plain English) what Array.map() does**

- function iterates over an array and runs a call back for each element. The callback receives the value and the index of the array element as a parameter.
- will always return you a new array of the same length as the original array comprised of your return values



2. **Describe (in plain English) what Array.reduce() does**

- iterates over an array and returns the last version of the “accumulator” … in each iteration, based on the value and/or idx of the current element in the array, you have the opportunity to modify and return the accumulator. After the last iteration of the array, that accumulator value is returned to the caller




3. **Provide code snippets showing how to use superagent() to fetch data from a URL and log the result**


- With normal Promise .then() syntax

`superagent.get(url).then(reult=>{consle.log(result)}.catch(err=>{consle.log(err)}`

- Again with async / await syntax

`let getData=async()=>{ let data=await superagent.get(url)consle.log(data.body)}; grtData();`


4. Explain promises as though you were mentoring a Code 301 level student

 - in java script the code run line by line (in order)
    and if there any function will take time the java script will skip it so for that we use promises we say to java script please finish this function i will wait and then you can go to the other lines 


5. Are all callback functions considered to be Asynchronous? Why or Why Not?

- callbacks don't have anything to do with the async concept at all. They're just regular functions, and they don't know or care whether they're going to be called asynchronously or not



[ref](https://dev.to/marek/are-callbacks-always-asynchronous-bah)