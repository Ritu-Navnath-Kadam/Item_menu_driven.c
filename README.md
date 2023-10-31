# Item_menu_driven.c
#include <stdio.h>

int main() {
    int ch, a = 0, ap = 0, b = 0, bp = 0, c = 0, cp = 0, t = 0, p = 0, D=0,r = 0, d = 0, db = 0, f = 0;

    do {
        printf("1. Bats\n");
        printf("2. Balls\n");
        printf("3. Books\n");
        printf("4. Exit\n");
        printf("Enter your choice: ");
        scanf("%d", &ch);

        switch (ch) {
            case 1:
                printf("Bats: ");
                scanf("%d", &a);
                printf("Bats price: ");
                scanf("%d", &ap);
                t = a * ap;
                printf("Total amount of bats = %d\n", t);
                if (a > 10)
                    d = t - t * 0.15;
                printf("The Discount on bats = %d\n", d);
                break;

            case 2:
                printf("Balls: ");
                scanf("%d", &b);
                printf("Balls price: ");
                scanf("%d", &bp);
                p = b * bp;
                printf("Total amount of balls = %d\n", p);
                if(b>10)
                D = p - p * 0.15;
                printf("The Discount on balls = %d\n", D);
                break;

            case 3:
                printf("Books: ");
                scanf("%d", &c);
                printf("Books price: ");
                scanf("%d", &cp);
                r = c * cp;
                printf("Total amount of books = %d\n", r);
                if(c>10 )
                db = r - r * 0.15;
                printf("The Discount on books = %d\n", db);
                break;

            case 4:
                f = t + p + r;
                printf("Total amount = %d\n", f);
                break;
            }
        } while (ch != 4);

    return 0;
}
