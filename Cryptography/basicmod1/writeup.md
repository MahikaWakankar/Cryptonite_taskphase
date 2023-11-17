# Description 
![Screenshot 2023-11-17 190029](https://github.com/MahikaWakankar/Cryptonite_taskphase/assets/148598677/2fee0fd2-41d3-490e-8a91-c43d1e4a304b)
As the numbers given were [350,63,353,198,114,369,346,184,202,322,94,235,114,110,185,188,225,212,366,374,261,213] we can find mod of the given numbers and map to the required letters and digits using the c code
#include <stdio.h>

// Function to calculate mod 37 of an array of numbers
void calculateMod37(int array[], int size) {
    for (int i = 0; i < size; i++) {
        array[i] = array[i] % 37;
    }
}

int main() {
    // Example array of numbers
    int numbers[] = {350,63,353,198,114,369,346,184,202,322,94,235,114,110,185,188,225,212,366,374,261,213};

    // Calculate mod 37 for the array
    int size = sizeof(numbers) / sizeof(numbers[0]);
    calculateMod37(numbers, size);

    // Display the results
    printf("Mod 37 of the array elements:\n");
    for (int i = 0; i < size; i++) {
        printf("%d ", numbers[i]);
    }

    return 0;
}
we get the mod numbers as 17 26 20 13 3 36 13 36 17 26 20 13 3 36 0 3 3 27 33 4 2 28, hence mapping to the required characters we get the flag as picoCTF{R0UND_N_R0UND_ADD17EC2}
