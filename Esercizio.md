# Gestione di una Biblioteca
## Libri

|   **Attributo**    | **Tipo di dato Java** | **Tipo di dato SQL** |                       Note                       |
| :----------------: | :-------------------: | :------------------: | :----------------------------------------------: |
|       Titolo       |        String         |       varchar        |                                                  |
|       Autore       |        String         |       varchar        |             Solo il nome dell'autore             |
|       Genere       |        String         |       varchar        |                                                  |
|       Pagine       |         short         |       smallint       |                                                  |
| Data Pubblicazione |       LocalDate       |         date         |                                                  |
|      Editore       |        String         |       varchar        |                                                  |
|   Disponibilità    |         short         |       smallint       |           Numero di copie disponibili            |
|        ISBN        |        String         |       varchar        |                   codice libro                   |
|     Copertina      |        String         |       varchar        | nome file o path generico all'immagine nel disco |
## Membri

|   **Attributo**    | **Tipo di dato Java** | **Tipo di dato SQL** |                Note                 |
| :----------------: | :-------------------: | :------------------: | :---------------------------------: |
|        Nome        |        String         |       varchar        |                                     |
|      Cognome       |        String         |       varchar        |      Solo il nome dell'autore       |
|  Data di nascita   |         Date          |      LocalDate       | Per eventuale verifica maggiore età |
| Telefono\Cellulare |        String         |       varchar        |                                     |
|       E-Mail       |        String         |       varchar        |                                     |
|     Indirizzo      |        String         |       varchar        |                                     |
## Prestiti
|   **Attributo**    | **Tipo di dato Java** | **Tipo di dato SQL** |                                 Note                                  |
| :----------------: | :-------------------: | :------------------: | :-------------------------------------------------------------------: |
| Data  del prestito |       LocalDate       |       DateTime       | Per sicurezza e controllo, può aver senso tener conto anche del tempo |
|      Scadenza      |       LocalDate       |         Date         |                                                                       |
|       Libro        |                       |                      |                     Riferimento alla entità Libro                     |
|       Membro       |                       |                      |                    Riferimento alla entità Membro                     |
# Catalogo di un Ristorante
## Piatti

| **Attributo** | **Tipo di dato Java** | **Tipo di dato SQL** |                                          Note                                          |
| :-----------: | :-------------------: | :------------------: | :------------------------------------------------------------------------------------: |
|     Nome      |        String         |       varchar        |                                    nome del piatto                                     |
|  Descrizione  |        String         |       varchar        |                                                                                        |
|   Categoria   |        String         |       varchar        |                              antipasto, primo, secondo...                              |
|    Prezzo     |        double         |       decimal        | potrebbero esserci piatti molto costosi in base al peso che possono andare oltre i 32k |
|   Immagine    |        String         |       varchar        |                         nome file o path generico all'immagine                         |
## Ingredienti
ipotizzo per gli ingredienti in magazzino

| **Attributo** | **Tipo di dato Java** | **Tipo di dato SQL** |            Note            |
| :-----------: | :-------------------: | :------------------: | :------------------------: |
|     Nome      |        String         |       varchar        |                            |
|   Scadenza    |       LocalDate       |         Date         |                            |
|   Categoria   |        String         |       varchar        |    frutta, verdura, ...    |
|   Quantità    |         short         |       smallint       | quantità disponibile in kg |
## Clienti
|   **Attributo**    | **Tipo di dato Java** | **Tipo di dato SQL** | Note |
| :----------------: | :-------------------: | :------------------: | :--: |
|        Nome        |        String         |       varchar        |      |
|      Cognome       |        String         |       varchar        |      |
|       E-mail       |        String         |       varchar        |      |
| Telefono\Cellulare |        String         |       varchar        |      |
# Catalogo di un Negozio di Fiori
## Fiori
| **Attributo** | **Tipo di dato Java** | **Tipo di dato SQL** |                                       Note                                        |
| :-----------: | :-------------------: | :------------------: | :-------------------------------------------------------------------------------: |
|     Nome      |        String         |       varchar        |                                                                                   |
|  Scientifico  |        String         |       varchar        |                            nome scientifico, opzionale                            |
|   Quantità    |         short         |       smallint       | non saprei che unità di misura associare concettualmente, immagino unità generica |
|    Prezzo     |        double         |       decimal        |                                                                                   |
|    Specie     |        String         |       varchar        |                                                                                   |
|   Immagine    |        String         |       varchar        |                      nome file o path generico all'immagine                       |
## Fornitori
|   **Attributo**    | **Tipo di dato Java** | **Tipo di dato SQL** | Note |
| :----------------: | :-------------------: | :------------------: | :--: |
|      Azienda       |        String         |       varchar        |      |
|     Indirizzo      |        String         |       varchar        |      |
|       E-Mail       |        String         |       varchar        |      |
| Telefono\Cellulare |        String         |       varchar        |      |
## Clienti
|   **Attributo**    | **Tipo di dato Java** | **Tipo di dato SQL** |                     Note                      |
| :----------------: | :-------------------: | :------------------: | :-------------------------------------------: |
|        Nome        |        String         |       varchar        |                                               |
|      Cognome       |        String         |       varchar        |                                               |
|       E-mail       |        String         |       varchar        |                                               |
| Telefono\Cellulare |        String         |       varchar        |                                               |
|     Indirizzo      |        String         |       varchar        | eventualmente necessario per qualche consegna |