# Lesson 3.1: Abstraction and Friends

## Resources

https://www.youtube.com/watch?v=Dxw9cIbzaLk

https://bjc.berkeley.edu/slides/BJC-L01-DG-Welcome-Abstraction.pdf

## Concepts

### Abstraction
Removing the specifics that are not relevant in a given context.

Examples

> Being able to drive a car without understanding how an internal combustion engine works or how an electric motor works.

> Being able to light a candle without knowing how matches work

### Detail removal

Reducing the complexity of an algorithm or process by focusing on the important parts.

The act or process of leaving out of consideration one or more properties of a complex object so as to attend to others.

### Generalization

Combining a group of related concepts or processes into a single principle/theory.

The process of formulating general concepts by abstracting common properties of instances.

Examples

You have a farm with many animal kinds. 
Different food for each animal 
You have directions that say 
	To feed dog, put dog food in dog dish 
	To feed chicken, put chicken food in chicken dish 
	To feed rabbit, put rabbit food in rabbit dish 
	Etc... 

How could you do better? 

> To feed <animal>, put <animal> food in <animal> dish 

You can think about your problem in terms of INPUTS you can use in place of concrete values.

If you want to make a program that calculates sine, you could precalculate every possible combination of inputs and outputs and return the ones that match, or ...

Use a function and do the calculation on the inputs.

```
y = sin(x)

instead of 

if 90.0 then 1.0
else if 30.0 then 0.5
else if 45.0 then 0.7071678

```

### Procedural decomposition

Breaking a problem down into smaller subtasks, usually to increase readability and/or maintainability, often by applying one of the above concepts.

> We have been doing this all along. We have been encouraging you to break down your problems into smaller parts that are easier to build and then work to expand that.

Examples:

Figuring out how to make a sprite accelerate in one direction before trying to randomize the direction.


## Activity 

Let's rethink the PB&J algorithm

Using these concepts, how can we abstract and decompose our PB&J problem?

To get started:

The act of spreading something spreadable on bread is the same no matter what spreadable thing you put on bread.

Make your improved solutions as concise as possible while still being easy to understand.

## Programming constructs

| Vocab | Definition |
| ----- | ---------- |
| Custom Blocks | Allow for one to make their own programming blocks. |
| Command Block | puzzle-piece shaped block that executes a command (it causes an effect).
| Reporter Block | Report a value, usually for use in another block's input slot. |
| Predicate Block | A hexagonal block that always returns a Boolean value (true or false). |
| Argument | Any area in a block that accepts user input, or another block. It could be a Boolean Block or a value placed inside of a variable or block. The value that is "passed into" a parameter of a custom block |
| Say Block |The block gives its sprite a speech bubble with the specified text — the speech bubble stays until an another speech or thought block is activated, or the stop sign is pressed. |