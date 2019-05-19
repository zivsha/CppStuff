#include <iostream>

class teller
{
public:
    teller()                                 { std::cout << "teller: Constructor"              << std::endl;               }
    ~teller()                                { std::cout << "teller: Destructor"               << std::endl;               }
    teller(const teller& rhs)                { std::cout << "teller: Copy Constructor"         << std::endl;               }
    teller(teller&& rhs) noexcept            { std::cout << "teller: Move Constructor"         << std::endl;               }
    teller& operator=(const teller& rhs)     { std::cout << "teller: Assignment Operator"      << std::endl; return *this; }
    teller& operator=(teller&& rhs) noexcept { std::cout << "teller: Move Assignment Operator" << std::endl; return *this; }
};

void by_value(teller t)            { std::cout << "by_value Called"      << std::endl; (void)t; }
void by_ref(teller& t)             { std::cout << "by_ref Called"        << std::endl; (void)t; }
void by_const_ref(const teller& t) { std::cout << "by_const_ref Called"  << std::endl; (void)t; }
void by_rvalue_ref(teller&& t)     { std::cout << "by_rvalue_ref Called" << std::endl; (void)t; }
