# wallace_multiplier

## Introduction:
The Wallace multiplier is another multiplication algorithm and architecture that offers advantages in terms of speed and area efficiency. It is named after American computer scientist Chris Wallace, who introduced it in the 1960s. The Wallace multiplier is an alternative to both classical multipliers and the Dadda multiplier.

The Wallace multiplier utilizes a reduction tree structure to perform multiplication. It reduces the number of partial products and levels in the tree, leading to a more compact and faster multiplier implementation. The key steps involved in the Wallace multiplier are as follows:

Partial Product Generation: Similar to other multiplication algorithms, the Wallace multiplier starts by generating the partial products by multiplying each bit of one number with each bit of the other number.

Grouping of Partial Products: The partial products are grouped into different levels based on their bit weights. Each level contains partial products with similar bit weights. The grouping is performed in a way that minimizes the number of partial products in each level.

Reduction Process: In the reduction process, each level of partial products is further reduced using a combination of compressors and carry-save adders. The compressors efficiently combine multiple partial products to form smaller sets of partial products, while the carry-save adders accumulate these sets to produce the reduced partial products.

Final Summation: The reduced partial products are finally summed up to obtain the final product. This can be done using a conventional adder structure, such as a carry-ripple adder or a carry-lookahead adder.

The Wallace multiplier offers advantages such as reduced hardware complexity, improved speed, and reduced power consumption compared to classical multipliers. By grouping the partial products and performing efficient reduction, it achieves a more compact multiplication structure with fewer levels and reduced critical path delay. This results in faster multiplication operations and reduced power dissipation.

Furthermore, the Wallace multiplier provides flexibility in terms of scalability, allowing for efficient multiplication of various operand sizes. It can handle different word lengths by adapting the grouping and reduction stages accordingly.

However, it's important to note that the performance and area efficiency of the Wallace multiplier may vary depending on the specific operand sizes and design constraints. Different optimizations, such as parallelization or the use of advanced adder structures, can be applied to further enhance its efficiency.

Overall, the Wallace multiplier is a powerful multiplication algorithm that balances speed, area efficiency, and scalability. It is commonly used in VLSI designs, particularly in applications that require high-speed multiplication and efficient hardware utilization.


### schematic

![image](https://github.com/sasi-kiran123/wallace_multiplier/assets/75782906/2f64bea8-183a-4aa3-b6da-3413a7083cee)



### Layout using Physical Design

![image](https://github.com/sasi-kiran123/wallace_multiplier/assets/75782906/14b079f7-bc50-43f0-a704-d0b11e0256bb)

