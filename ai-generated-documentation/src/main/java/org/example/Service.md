![Capgemini Logo](https://www.capgemini.com/wp-content/themes/capgemini2020/assets/images/logo.svg)

### Make it real.

---
## Dokumentacja kodu źródłowego Service.java

**Overview:** 

Kod źródłowy `Service.java` definiuje klasę `Service`, która zawiera dwie metody: `isEven` i `highComplexityMethod`. Metoda `isEven` sprawdza, czy podany argument jest liczbą parzystą, zwracając wartość logiczną (true lub false). Metoda `highComplexityMethod` wykonuje złożoną logikę warunkową na podstawie trzech argumentów całkowitych.

**Package/module name:** org.example

**Class/file name:** Service.java

**Detailed Documentation:**

* **Class: Service**
    *   Description: Klasa `Service` zawiera metody pomocnicze do sprawdzania parzystości liczby i wykonywania złożonej logiki warunkowej. 

* **Method: isEven(int input)**
    *   Description: Metoda `isEven` sprawdza, czy podany argument (`input`) jest liczbą parzystą.
    *   Parameters:
        *   `input`: Liczba całkowita, której parzystość ma być sprawdzona.
    *   Return Values:
        *   `boolean`: Zwraca `true`, jeśli `input` jest liczbą parzystą, w przeciwnym razie zwraca `false`.

* **Method: highComplexityMethod(int a, int b, int c)**
    *   Description: Metoda `highComplexityMethod` wykonuje złożoną logikę warunkową na podstawie trzech argumentów całkowitych (`a`, `b`, `c`). Wyświetla komunikaty tekstowe w konsoli informujące o wartościach argumentów.
    *   Parameters:
        *   `a`: Liczba całkowita.
        *   `b`: Liczba całkowita.
        *   `c`: Liczba całkowita.

**Pseudo Code:**


```
# Klasa: Service

# Metoda: isEven(input)
  1. Oblicz resztę z dzielenia input przez 2.
  2. Jeśli reszta jest równa 0, zwróć true (input jest liczbą parzystą).
  3. W przeciwnym razie, zwróć false (input nie jest liczbą parzystą).

# Metoda: highComplexityMethod(a, b, c)
  1. Sprawdź wartość a:
     - Jeśli a jest równe 0:
       - Sprawdź wartość b:
         - Jeśli b jest większe od 0:
           - Sprawdź wartość c:
             - Jeśli c jest większe od 0, wyświetl "c is positive".
             - W przeciwnym razie, wyświetl "c is non-positive".
         - W przeciwnym razie, wyświetl "b is non-positive".
     - Jeśli a jest mniejsze od 0:
       - Sprawdź wartość b:
         - Jeśli b jest większe od 0:
           - Sprawdź wartość c:
             - Jeśli c jest większe od 0, wyświetl "c is positive".
             - W przeciwnym razie, wyświetl "c is non-positive".
         - W przeciwnym razie, wyświetl "b is non-positive".
     - W przeciwnym razie (a nie jest równe 0 ani mniejsze od 0), wyświetl "a is non-positive".



```




