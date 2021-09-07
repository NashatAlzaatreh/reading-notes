# FUNCTIONAL PROGRAMMING

## Functional Programming Concepts

### - What is functional programming?

#### Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

### - What is a pure function and how do we know if something is a pure function?

#### A pure function is a function which:

#### - It returns the same result if given the same arguments (it is also referred as deterministic) and it does not cause any observable side effects

### - What are the benefits of a pure function?

#### Pure functions are much easier to read and reason about. All relevant inputs and dependencies are provided as parameters, so no effects are observed that alter variables outside of the set of inputs. This means that we can quickly understand a function and its dependencies, just by reading the function’s declaration.

### - What is immutability?

#### Unchanging over time or unable to be changed

### - What is Referential transparency?

#### variable having the same value without changing the result of the program. As a result, methods should always return the same value for the given argument without any side effects

## Node JS Tutorial for Beginners #6 - Modules and require()

### - What is a module?

#### any of a number of distinct but interrelated units from which a program may be built up or into which a complex activity may be analysed.

### - What does the word ‘require’ do?

#### How do we bring another module into the file the we are working in? we need to import the module. we will use the require keyword at the top of the file. The result of require is then stored in a variable which is used to invoke the functions using the dot notation

### - How do we bring another module into the file the we are working in?

#### we need to import the module. we will use the require keyword at the top of the file. The result of require is then stored in a variable which is used to invoke the functions using the dot notation

### - What do we have to do to make a module available?

#### we need to export whatever we need to available outside the module
