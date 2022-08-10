# Control-task

Контрольная работа по итогам вводной четверти на курсе GB.
В рамках контрольной работы создан репозиторий, составлена блок-схема и написан код для решения задачи.

Описание кода задачи:
https://replit.com/@OlgaKor/Ctask#main.cs

using System;

class Program {
  public static void Main (string[] args) {
    string[] Array1 = new string[7] {"Hello", "It", "is", "been", "ok", "!!!!", ":-)"};
    string[] Array2 = new string[Array1.Length];
    int number = 0;
    void SecondArray(string[] Array1, string[] Array2)
      {
       int number = 0;
       for (int i = 0; i < Array1.Length; i++)
         {
         if(Array1[i].Length <= 3)
           {
           Array2[number] = Array1[i];
           number++;
           }
         }
      }
    void PrintArray(string[] Array)
      {
      for (int i = 0; i < Array.Length; i++)
        {
         Console.Write($"{Array[i]} ");
        }
      Console.WriteLine();
      }
    SecondArray(Array1, Array2);
    PrintArray(Array2);
  }
}
