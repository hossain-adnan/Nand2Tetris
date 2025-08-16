# And Gate Thought Process

## And gate logic
- If `a = 1` and `b = 1` → `out = 1`  
- Else → `out = 0`

## Truth Table for And 
| x | y | out |
|---|---|-----|
| 0 | 0 |  0  |
| 0 | 1 |  0  |
| 1 | 0 |  0  |
| 1 | 1 |  1 |

## Truth Table for Nand (used to build Not)
| x | y | out |
|---|---|-----|
| 0 | 0 |  1  |
| 0 | 1 |  1  |
| 1 | 0 |  1  |
| 1 | 1 |  0  |

## Observation
- `Nand(a,b) = Not(And(a,b))`  
- `Not(Nand(a,b)) = Not(Not(And(a,b))) = And(a,b)`

## Implementation in HDL
```hdl
Nand(a=a , b=b , out=aNandb);
Not(in=aNandb, out=out);
