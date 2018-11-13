# sesion7-tarea-individual

Part 1: Web Services SOAP amb objectes

Volem crear un webservice SOAP per consultar les notes dels alumnes.

1- Per tal de gestionar les notes dels alumnes heu de dissenyar les següents classes, amb getters, setters i constructors:

Classe Nota: Ens servirà per representar la nota de cada assignatura.
Té les  propietats:
IdAssignatura: Identificador de l'assignatura
NomAssignatura: Nom de l'assignatura
Nota: Valor numèric de la nota entre 1 i 10

Classe Alumne: Ens servirà per representar la informació dels alumnes.
Té les propietats:
id: Identificador de l'alumne
nom: Nom de l'alumne
dni: dni de l'alumne
notes : llista de notes de l'alumne  (List<nota>)

2- Crearem el webservice SOAP WSalumnes que tindrà els següents mètodes:

getAlumnes()

–	Retornarà una llista d'alumnes.
–	Es tracta només d'una simulació. En aquest cas podem crear objectes de tipus alumne des del propi mètode i afegir-los a una llista.

getNotes(int idalumne)

–	Retornarà una llista de notes.
–	Com en el mètode anterior simularem que retornem les notes d'un alumne. En aquest cas ha de simular almenys dos notes diferents depenent del paràmetre idAlumne. Per crear el butlletí crearem al codi els objectes alumne i una llista de nota que afegirem a un objecte notes.

3- Crearem una aplicació client que consultarà dades al webservice. Aquesta aplicació tindrà les següents funcionalitats:

1)	Llistar Alumnes: Cridarà al webservice per tal d'obtenir una llista d'alumnes i la mostrarà per pantalla.
2)	Rebre notes alumne: Demanarà l'ID d'un alumne i farà la crida al webservice per obtindre les notes d'aquest alumne. Mostarà les dades de l'alumne i les seves notes per pantalla.

Part 2: WebService + JAXB

En aquesta segona part ampliarem l'exercici anterior per tal de que el WebService no simuli les dades, sinó que les carregui de fitxers XML que representin la informació dels alumnes i les seves notes mitjançant la desserialització  d'objectes (Unmarshaling) amb JAXB.

Tindrem un fitxer XML per cada: 1. alumne, 2.xml ... que contindrà les dades i les notes de l'alumne.
Heu de decidir quina estructura ha de tindre cada fitxer per a poder convertir-lo a objecte.

Part 2: WebService + JAXB

En aquesta segona part ampliarem l'exercici anterior per tal de que el WebService no simuli les dades, sinó que les carregui de fitxers XML que representin la informació dels alumnes i les seves notes mitjançant la desserialització  d'objectes (Unmarshaling) amb JAXB.

Tindrem un fitxer XML per cada: 1. alumne, 2.xml ... que contindrà les dades i les notes de l'alumne.
Heu de decidir quina estructura ha de tindre cada fitxer per a poder convertir-lo a objecte.
