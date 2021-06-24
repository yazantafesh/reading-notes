# Node Ecosystem, TDD, CI/CD

1. Describe (in plain English) what Array.map() does.

    Creates a new array with the results of calling a function for every array element. The map() method calls the provided function once for each element in an array, in order.

2. Describe (in plain English) what Array.reduce() does.

    Used to reduce the array to a single value and executes a provided function for each value of the array (from left-to-right) and the return value of the function is stored in an accumulator.

3. Provide code snippets showing how to use superagent() to fetch data from a URL and log the result:

    - **With normal Promise .then() syntax.**

        ```
        superagent.get(`https://swapi.dev/api/people`).then(data=>{
            data.body.results.forEach(item=>{
         console.log({[item.name] : item.url})
           })
        }).catch(error=>console.log(error));
        ```

    - **Again with async / await syntax.**

        ```try{
           let data=await superagent.get(`https://geocode.xyz/${city}?json=1`);
           console.log(city,data.body.longt,data.body.latt)
           }catch(error){console.log(error)}```

4. Explain promises as though you were mentoring a Code 301 level student.

    A **Promise** is a proxy for a value not necessarily known when the promise is created. It allows you to associate handlers with an asynchronous action’s eventual success value or failure reason.

    The methods promise.then(), promise.catch(), and promise.finally() are used to associate further action with a promise that becomes settled.

5. Are all callback functions considered to be Asynchronous? Why or Why Not?

    Not necessarily. An asynchronous function means that one function’s actions do not need to be completed for the next function to run. While you can structure a callback in this way, it is also possible to have callback functions that run that are dependent on the result of a previous function.
