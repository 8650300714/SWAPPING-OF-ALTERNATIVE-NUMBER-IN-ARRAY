# SWAPPING-OF-ALTERNATIVE-NUMBER-IN-ARRAY
#include <iostream>
using namespace std;

int main() {
    int num, arr[100];
    
    cout << "Enter the size of the array: ";
    cin >> num;
    
    cout << "Enter elements of the array: " << endl;
    for (int i = 0; i < num; i++) {
        cout << "Element " << i + 1 << ": ";
        cin >> arr[i];
    }
    
    // Swap alternate elements
    for (int i = 0; i < num - 1; i += 2) {
        int temp = arr[i];
        arr[i] = arr[i + 1];
        arr[i + 1] = temp;
    }
    
    // Print the swapped array
    cout << "Array after swapping alternate elements: ";
    for (int i = 0; i < num; i++) {
        cout << arr[i] << " ";
    }
    cout << endl;
    
    return 0;
}
