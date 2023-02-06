# Activities

## Task 1/3: Divide-and-conquer

The code in `./src/pow1.cpp` and `./src/pow2.cpp` compute the power `pow(x, n)` using iterative and recursive approaches respectively.

> Refer to the following [link](https://www.techiedelight.com/power-function-implementation-recursive-iterative/).

- What is the time complexity for both approaches?

## Task 2/3: Divide-and-conquer vs Decrease and conquer

- In many literature, Binary search is referred to use divide-and-conquer technique. Discuss in groups whether you agree or disagree and justify your answers. Refer to the the following thread: [Why Binary Search is not a divide and conquer algorithm?](https://stackoverflow.com/questions/8850447/why-is-binary-search-a-divide-and-conquer-algorithm)

DnC algorithms have a few general/common properties; they:
divide the original problem instance into a set of smaller sub-instances of itself;
independently solve each sub-instance;
combine smaller/independent sub-instance solutions to build a single solution for the larger/original instance
The Binary Search does not really even generate a set of independent sub-instances to be solved, as per step 1; it only simplifies the original problem by permanently discarding sections it's not interested in. In other words, it only reduces the problem's size and that's as far as it ever goes.

A DnC algorithm is supposed to not only identify/solve the smaller sub-instances of the original problem independently of each other, but also use that set of partial independent solutions to "build up" a single solution for the larger problem instance as a whole.

## Task 3/3: Individual, at home

- Refactor the code in `./src/pow2.cpp` to optimize the time complexity of the recursive approach. Use `./src/pow3.cpp` as a starter.
- Refactor the code in `pow1.cpp` and `pow2.cpp`, as follows:
  - Replace `printf()` with` std::cout()`
  - Include the right headers e.g. `iostream`

## Links

- https://www.techiedelight.com/power-function-implementation-recursive-iterative/
- https://cpp.sh/
