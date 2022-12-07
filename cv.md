1. Pavel Sushko 
2. phone number (mts.by): +375295999886, tg: @pvell, inst: @p.velll
3.I am a first-year student of BSU (rfikt), I study programming in the specialty computer security, 
I have been programming (c++) for 3 months and I see myself in this field.
 I entered the courses in order to study programming a little deeper than they give at uni. 
I have a strong desire to work in an IT company and I strive for this.
4. performing programming tasks is my entire work experience. here is an example code (c++):
#include <iomanip>
#include <iostream>
#include <cstdlib>
#include <stdlib.h>
enum ARRAY_USER_INPUT
{
    WORK_WITH_DEFAULT_MATRIX = 1,
    WORK_WITH_RANDOM_MEMBERS,
    WORK_WITH_USER_INPUT_MEMBERS,
};
using namespace std;

 const int M = 3, N = 3;


void summary( int a[M][N] )
{
    int sum = 0;
    int min = a[0][0];
    int k = 0;
    int l = 0;

    cout << "summary of column elements:";
    for (int i = 0; i < M; i++)
    {
        for (int j = 0; j < N; j++)
        {
            if (min > a[i][j])
            {
                min = a[i][j];
                if (min <= a[i][j+1]  min <= a[i+1][j])
                k = i; 
                if (k >= 0 && k < N)
                {

                    for (int i = 0; i < M; i++)
                        sum += a[i][k];
                    cout << sum << endl;

                    
                }

            }
            break;
        }
    }

}
void default_matrix( int a[M][N])
{

    cout << "matrix:" << endl;
    // вывод матрицы в виде таблицы
    for (int i = 0; i < M; i++)
    {
        for (int j = 0; j < N; j++)
            cout << setw(3) << a[i][j]; // инициализация массива при объявлении
        cout << endl;
    }
    
    
}
void random_matrix( int a[M][N])
{
    for (int i = 0; i < M; i++)
        for (int j = 0; j < N; j++) // заполнение случайными
            a[i][j] = rand() % 100; // числами 0..99
    for (int i = 0; i < M; i++)
    {
        for (int j = 0; j < N; j++)
            cout << setw(3) << a[i][j];
        cout << endl;
    }
    
    
}

void user_input_matrix( int a[M][N])
{
    cout << "input your array:" << endl;

    for (int i = 0; i < M; i++)
        for (int j = 0; j < N; j++) // значения элементов 
            cin >> a[i][j]; // матрицы вводятся с
    // клавиатуры
    for (int i = 0; i < M; i++)
    {
        for (int j = 0; j < N; j++)
            cout << setw(3) << a[i][j];
        cout << endl;
    }
    cout << endl;
    
    
}


int main()
{
    int num_way;
    cout << "select the way of fulfilment:" << endl;
    cout << "enter '1' if you want to work with ready array;" << endl;
    cout << "enter '2' if you want to work with random members of array;" << endl;
    cout << "enter '3' if you want to work with array;" << endl;
    cin >> num_way;
    int a[M][N] = { { 7, 5, 2},
        { 6, 7, 8},
        {12,13,14}
    };
    if (num_way == 1) {
        default_matrix( a);
        summary( a);
    }

    if (num_way == 2)
    {
        random_matrix( a);
        summary( a);
    }
    if (num_way == 3)
    {
        user_input_matrix( a);
        summary( a);
    }
    



    cout << "numbers of monotonically increasing lines:";

    if (num_way == 1  num_way == 3) {
        int j = 0;
        for (int i = 0; i < M; i++)
        {
            if (a[i][j] < a[i][j + 1])
            {
                cout << j + 1 << " ";
            }
            j++;

        }
    }
    if (num_way == 2) {
        cout << "  there isn't monotonically increasing lines";
    }

    return 0;
}
5. I have not taken courses and trainings with js, I will get to know myself)
6.Officially, my English level is B 1, 
I have experience of communicating with Americans, my neighbor is from America,
 we often went fishing with him, in general, 
I often stayed with him. It was he who made me understand that programming is cool