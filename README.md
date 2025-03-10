
    
    #include <iostream>
    #include <cmath>

    int main() {
        int n;
        std::cout << "Ingrese un entero n: ";
        std::cin >> n;
    
        int sum_of_cubes = 0;
        for (int i = 1; i <= n; i++) {
            sum_of_cubes += std::pow(i, 3);
        }

    
        int formula_result = std::pow((n * (n + 1)) / 2, 2);

    
        std::cout << "Suma de los cubos: " << sum_of_cubes << std::endl;
        std::cout << "Resultado de la fórmula: " << formula_result << std::endl;

        if (sum_of_cubes == formula_result) {
            std::cout << "Los valores coinciden." << std::endl;
        } else {
            std::cout << "Los valores no coinciden." << std::endl;
        }

        return 0;
        }

