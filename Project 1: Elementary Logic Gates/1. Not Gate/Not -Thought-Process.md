# Not Gate Thought Process

## Not gate logic
- If `in = 1` → `out = 0`  
- Else `out = 1`

## Truth Table for Not
| in | out |
|----|-----|
| 0  |  1  |
| 1  |  0  |

## Truth Table for Nand (used to build Not)
| x | y | out |
|---|---|-----|
| 0 | 0 |  1  |
| 0 | 1 |  1  |
| 1 | 0 |  1  |
| 1 | 1 |  0  |

## Example
- `Not(1) = 0 ` 
- `Nand(1,1) = 0`  
- `Nand(x,x) = 0 ` 

## Implementation in HDL
```hdl
Nand(a=x, b=x, out=out);
