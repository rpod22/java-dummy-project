![Capgemini Logo](https://www.capgemini.com/wp-content/themes/capgemini2020/assets/images/logo.svg)

### Make it real.

---
## Dokumentacja kodu źródłowego Client.java

**Overview:** 

Kod źródłowy `Client.java` definiuje klasę `Client`, która implementuje proste pozdrowienie dla podanego imienia. Klasa ta korzysta z usługi `Service` (nie pokazanej w kodzie) do sprawdzenia parzystości długości imienia i generowania odpowiedniego powitania.

**Package/module name:** org.example

**Class/file name:** Client.java

**Detailed Documentation:**

* **Class: Client**
    *   Description: Klasa `Client` reprezentuje klienta, który wysyła żądanie o pozdrowienie z podanym imieniem. 
    *   Fields:
        *   `service`: Obiekt typu `Service`, używany do sprawdzania parzystości długości imienia.

* **Constructor: Client(Service service)**
    *   Description: Konstruktor klasy `Client`, który inicjalizuje pole `service`.
    *   Parameters:
        *   `service`: Obiekt typu `Service`, używany do sprawdzania parzystości długości imienia.

* **Method: greeting(String name)**
    *   Description: Metoda `greeting` generuje pozdrowienie dla podanego imienia. 
    *   Parameters:
        *   `name`: String, imię osoby, dla której ma zostać wygenerowane pozdrowienie.
    *   Return Values:
        *   String, pozdrowienie w postaci "Hello, [name]". Jeśli długość imienia jest parzysta, powitanie jest wyświetlane z dużej litery.
    *   Important Logic:
        1. Sprawdza, czy podane imię nie jest `null` ani puste. W przypadku braku lub pustych danych rzuca wyjątek `IllegalArgumentException`.
        2. Wywołuje metodę `isEven` z obiektu `service`, aby sprawdzić parzystość długości imienia.
        3. Tworzy ciąg "Hello, %s" i formatuje go z podanym imieniem.
        4. Jeśli długość imienia jest parzysta, zwraca powitanie w formacie wielkiego pisma. W przeciwnym razie zwraca standardowe pozdrowienie.

**Pseudo Code:**


```
# Klasa: Client

# Metoda: greeting(name)
  1. Sprawdź, czy name nie jest null ani pustym ciągiem znaków.
     - Jeśli tak, rzuć wyjątek IllegalArgumentException z komunikatem "Name cannot be null or empty".
  2. Wywołaj metodę isEven z obiektu service, przekazując długość imienia jako argument.
  3. Stwórz ciąg "Hello, %s" i sformatuj go z podanym imieniem.
  4. Jeśli wynik metody isEven jest true (długość imienia jest parzysta):
     - Zwróć sformatowany ciąg w formacie wielkiego pisma.
  5. W przeciwnym razie:
     - Zwróć sformatowany ciąg bez zmiany formatu. 


```



