you can take the source and improve or you can just claim its your yours idrc
just know your a skid ez L

Source Code

#include <iostream>
#include <iomanip>

void simulateGrowth(double value1, double value2, double multiplier, double target) {
    std::cout << "CPS Value   | Click Duty" << std::endl;
    std::cout << "------------------------" << std::endl;
    while (value1 < target || value2 < target) {
        if (value1 < target) value1 *= multiplier;
        if (value2 < target) value2 *= multiplier;
        std::cout << std::fixed << std::setprecision(4)
            << std::setw(10) << value1 << " |" << std::setw(10) << value2 << std::endl;
    }
}

int main() {
    std::cout << "Growth Simulation" << std::endl;
    double value1 = 3.78;
    double value2 = 2.72;
    double multiplier = 1.01;
    double target = 24;

    simulateGrowth(value1, value2, multiplier, target);

    // Wait for user to press any key before exiting
    std::cout << "Press Enter to close...";
    std::cin.ignore(); // Ignore leftover newline
    std::cin.get(); // Wait for key press

    return 0;
}
