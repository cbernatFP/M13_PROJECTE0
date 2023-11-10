# M13_PROJECTE0

## Exemple Bàsic JPA CRUD. Projecte Book.
### Què farem
La nostra aplicació tindrà bàsicament les següents classes:
- ProjecteDamDawApplication.java. Defineix l’aplicació SpringBoot...
- Book.java. JPAEntity. L’objecte/entitat que consultem. I que voldrem fer “persistent”.
  - BookRepository.java. Extendrà CRUDRepository o JPARepository. Defineix els mètodes d’accés a la base de dades (o a la capa de persistència).
  - els mètodes add, borrar, modifica que vam fer amb l’ArrayList ja estarien implementats a CRUDRepository. Que a més, no els inserta, llegeix o esborra d’una llista, sinó d’una BD. No els haurem de crear. Els podem fer servir directament.
  - JPA és un ORM. Mapeja estructures d’una BD relacional a objectes Java.
- En aquest cas només farem el llistat de llibres findAll
- BookController.java. Exposa els mètodes que permeten connectar-se a l’aplicació a través de crides http. En aquest cas NOMÉS llistarem els llibres
