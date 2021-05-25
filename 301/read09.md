# Functional Programming Concepts

1. What is functional programming?

    Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

2. What is a pure function and how do we know if something is a pure function?

    The first fundamental concept we learn when we want to understand functional programming is pure functions. But what does that really mean? What makes a function pure?

    So how do we know if a function is pure or not? Here is a very strict definition of purity:

    - It returns the same result if given the same arguments (it is also referred as deterministic).

    - It does not cause any observable side effects

3. What are the benefits of a pure function?

    The code’s definitely easier to test. We don’t need to mock anything.

4. What is immutability?

    Unchanging over time or unable to be changed.

5. What is Referential transparency?

    Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

# Node JS Tutorial for Beginners #6 - Modules and require()

1. What is a module?

    Module in Node. js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node. js application. Each module in Node. js has its own context, so it cannot interfere with other modules or pollute global scope.

2. What does the word ‘require’ do?

    The builtin require function is the easiest way to include modules that exist in separate files. The basic functionality of require is that it reads a JavaScript file, executes the file, and then proceeds to return the exports object.

3. How do we bring another module into the file the we are working in?

    To access the module functions, we have to export the functions and import them in the file we want to call the functions.

    To include functions defined in another file in Node.js, we need to import the module. we will use the require keyword at the top of the file.

    The result of require is then stored in a variable which is used to invoke the functions using the dot notation.

    To see that in action, let’s import the lib.js module by requiring it inside the main.js file and invoke the add() function with dot notation.

4. What do we have to do to make a module available?

    Export it using the add() function in the lib.js file.

## Things I want to know more about

handling modules in Node.js
