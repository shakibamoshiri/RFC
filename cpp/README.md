## Regex Function Collection

### Some useful functions to deal with Regular Expressions; All written by standard library.
```C++
#include <regex>
#include <string>
#include <vector>
#include <iterator>
#include <algorithm>
```

Just: `include <rfc.hpp>`

### Examples:

#### regex_is_valid:
```C++
int main(){

    const char* r = k5::regex_is_valid( "/\/\/\\" ); // regex_is_valid (2)
    if( r ){
        std::cout << "not valid regex\n";
        std::cout << "because: " << r << '\n';
    } else {
        std::cout << "okay\n";
    }


return 0;}

/* the output:

not valid regex
because: Unexpected end of regex when escaping.

*/
```