# Math computing layer for Interactive calculators and Interactive learning enviroment

## Implements

### Layers

- **EquationSolver** - solves universal equation fastly as it can, only for speed computing (can solves even systems of equations)
- **EquationSymplifier** - Tries to find patterns in equation to make it as simple as possible
- **EquationSolveHelper** - solves equation in different ways, make the solving simple as possible + writes the whole way how to solve 
- **EquationGenerator** - generates equations by editable and modificable templates, can use Simplifier to make it easier to solve then
- **EquationAnalyser** - analyse equation solve input, can find wrong operations and give advices how to compute better
- **FunctionCalc** - can computes with function, for ex.: integrals, derivates, etc
- **FunctionPlotter** - plots or shows table of entered functions, can be used as graphic calculator
- **StatementCalc** - statement calculator, works with intervals, booleans and sets
- **StatementGenerator** - statement example generator

#### Later on / further features

- **MathExplainer** - explains math symbols and topics with many ways
- **MathTrainer** - your personal math-experience trainer/mentor, analyses what you can/can't in math

#### Unvisible layers

- **EquationTokenizer** - transfer string equation to tokenized tree (RPN)
- **StatementTokenizer** - transfer string statement to tokenized tree

### Algebra

- Numbers
	- Real
	- Natural
	- Integers
	- Irational
	- Complex
	- Basic operations
	- Fractions
- Sets 
	- Finite
	- Infinite
	- Intersection
	- Unification
	- Get if elements is part
	- Setting by condition or list of values
- Intervals
- Equations
- Inequalities
- Statements
	- Booleans
	- Boolean algebra
	- Opearators
- Functions
	- Plotting
	- Derivates
	- Integrals
- Sumary (add n times the expression)
- Numerizator (multiply n times the expression)

## Math types in parser

- variables 
  - Linear (ax)
  - Quadratic (ax^2)
  - Irational (sqrt(ax,n))
  - Polynomial (ax^n)
  - Complex (a, bi)
- Constants
  - fractions
  - numbers
  - math constants(e, pi...)

### Objects

- Equation
- List of elements
- Statement
- System of equations


## TODO

- add complex numbers
- Safe numerics, overflow checking: [Boost docs](https://www.boost.org/doc/libs/1_81_0/libs/safe_numerics/doc/html/index.html)