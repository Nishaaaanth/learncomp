# DSA

## Basics
### Even or Odd
```c
if( num & 1) {
    return "even";
}
```

### Number System
- Bin to Hex => group 4 bin and convert since 1111 is F.
- Bin to Oct => group 3 bin and convert since 111 is 7.
- Bin to Dec => divide by 2 and place in reverse.

```c
// For conversion of digits take digits value instead of having if clauses
std::string digits = "0123456789ABCDEF";

// For assigning max number of bit limit to represent unsigned int in bits
std::bitset<std::numeric_limits<unsigned int>::digits> bin(number);
```

#### Conversion to string
```c
std::to_string()
```

### Vector Init
```c
std::vector<int> v(n, -1);
```

### Map
```c
std::map<int, ll> dict;

std::map<int, ll>::iterator it = dict.find(n);

it.first = key;
it.second = value;
```

### Calculation Tip
- Always if there are exponent calculation and division please divide the number as soon as the exponent calc or split the exponent and divide one term and then divide the other term with the split denominator. This can be used to avoid overflows during formula usecase like
```c
n*(n+1)*(2n+1)/6;

(n*(n+1)/2)*(2*n+1)/3;
```

### Reverse (Recurse) -> Do again
### Power Check (log(N)) -> Do again
### Overlapping Rectangle -> Do again
### GCD -> Do again
### isPerfect -> Do again
### Calendar Problems -> Learn the concept
### Fibonacci -> Learn all the methods

### prime
```c
6k-1 or 6k+1
```

### Power check
```c
log(x)/log(y);
```

### Distance Calculation gives out floating point number
```c
static_cast<int> //instead of (x*1.0)

//or round it out
round()
```

### Bitwise Logic
```c
n&1  // n%2 => checks the least significant bit. If it's 1 it's odd if not it's even
n>>1 // n/2 => shifts the value to the right by 1 bit thereby reducing the value by 2
n<<2 // n*2 => shifts to left meaning multiplying by 2

```
