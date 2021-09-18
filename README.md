#include <stdio.h>

void swap_pointers(int *n1, int *n2) {
    int temp = *n1;
    *n1 = *n2;
    *n2 = temp;
}

int main() {
    int n1, n2;
    printf("Enter two integers: ");
    scanf("%d", &n1);
    scanf("%d", &n2);

    printf("%d %d\n", n1, n2);
    swap_pointers(&n1, &n2);
    printf("%d %d\n", n1, n2);
    return 0;
}
