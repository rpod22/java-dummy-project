![Capgemini Logo](https://www.capgemini.com/wp-content/themes/capgemini2020/assets/images/logo.svg)

### Make it real.

---
## Dokumentacja skryptu `pom.xml`

**1. Przegląd:**

Skrypt `pom.xml` jest plikiem konfiguracyjnym dla narzędzia budowania Maven, używanego do zarządzania zaleznościami, kompilacji i testowania projektu Java. 

**2. Narzędzie budujące:** Maven

**3. Nazwa skryptu/pliku:** `pom.xml`

**4. Szczegółowa dokumentacja:**

* **Sekcja: `<properties>`**:
    *   Opis: Definiuje właściwości używane w pliku `pom.xml`.
    *   Parametry:
        *   `maven.compiler.source`: Wersja języka Java, która będzie używana do kompilacji kodu źródłowego (17).
        *   `maven.compiler.target`: Wersja języka Java, na którą zostanie skompilowany kod (17).
        *   `project.build.sourceEncoding`: Kodowanie znaków używane w projekcie (UTF-8).
        *   `junit.jupiter.version`: Wersja biblioteki JUnit Jupiter używana do testowania (5.10.0).

* **Sekcja: `<dependencies>`**:
    *   Opis: Definiuje zależności projektu, czyli biblioteki zewnętrzne, których kod jest potrzebny do działania aplikacji.
    *   Parametry: Każda zależność ma następujące parametry:
        *   `groupId`: Identyfikator grupy, do której należy biblioteka (np. `org.mockito`).
        *   `artifactId`: Nazwa artefaktu (np. `mockito-core`).
        *   `version`: Wersja biblioteki (np. `5.6.0`).
        *   `scope`: Zakres użycia zależności (np. `test` - używana tylko do testów).

* **Sekcja: `<build>`**:
    *   Opis: Definiuje konfigurację procesu budowania projektu, w tym pluginy Maven używane do wykonywania zadań budowania.
    *   Parametry:
        *   `<plugins>`: Lista pluginów Maven używanych w procesie budowania.

* **Sekcja: `<plugin>`**:
    *   Opis: Definiuje pojedynczy plugin Maven.
    *   Parametry:
        *   `groupId`: Identyfikator grupy, do której należy plugin (np. `org.apache.maven.plugins`).
        *   `artifactId`: Nazwa artefaktu (np. `maven-surefire-plugin`).
        *   `version`: Wersja pluginu (np. `3.0.0`).

**5. Wersja języka:** Java 17

**6. Wersje zależności:**

*   Mockito: 5.6.0
*   AssertJ: 3.24.2
*   JUnit Jupiter Engine: 5.10.0
*   JUnit Jupiter API: 5.10.0
*   Mockito JUnit Jupiter: 5.6.0

**7. Pseudokod:**

```
# Proces budowania projektu z pom.xml

1.  Wczytaj plik `pom.xml`.
2.  Pobierz właściwości z sekcji `<properties>`, takie jak wersje języka Java i biblioteki JUnit Jupiter.
3.  Pobierz listę zależności z sekcji `<dependencies>`.
4.  Dla każdej zależności:
    - Pobierz informacje o grupie, nazwie artefaktu, wersji i zakresie użycia.
    - Pobierz zależność z repozytorium Maven.
5.  Pobierz pluginy budowania z sekcji `<plugins>`.
6.  Wykonaj zadania budowania określone przez pluginy:
    - Kompilacja kodu źródłowego Java do klas.
    - Uruchomienie testów jednostkowych za pomocą JUnit Jupiter i Mockito.

7.  Utwórz pakiet aplikacji z skompilowanymi klasami i wynikami testów.



```


**8. Odpowiedniki zależności i pluginów:**

*   Maven: Gradle, npm (dla JavaScript)
*   Mockito: Jest (Python), Sinon.js (JavaScript)
*   AssertJ: Chai (JavaScript), pytest (Python)
*   JUnit Jupiter: TestNG (Java), Mocha (JavaScript)



