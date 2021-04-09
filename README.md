# Sorted Linked List

## Implementation
Your task is to implement a sorted linked list. The elements must
be inserted at the correct position. Inserting at the last position
and sorting afterwards **is not** allowed.

A basic skeleton is already provided. The generic interface
`SortedList` is the base of your implementation. Therefore, 
`SortedLinkedList` must implement it. Add generics to that class.
`SortedLinkedList` should also implement a good-looking `toString()`
method.

An output example could be:
~~~
| a | ->| b | ->| g | ->| x | ->| z | 
~~~

The goal is to have a list which can work with all comparable
elements.

## Testing
Test your implementation intensively. Try out corner cases. 
Test all your methods = 100% code coverage.
Your implementation must care of error handling. Moreover, test
it with at least three different classes.
* One of them should be String.
* Two self written classes which are comparable. Small classes are
totally fine.
  
## Questions
* How can you change the ordering of the list? From ascending 
to descending. Name at least two different methods.
- Collections.sort(list);
- Collections.reverse(list);
- compare to Methode

* Can the inner Node class be static? Justify your answer.
- Ja, eine innere Klasse ist einer Instanz ihrer oberen Klasse zugeordnet und hat direkten Zugriff auf die Methoden und Felder dieses Objekts. 

* Can you name the generic placeholder `Placeholder` instead of
`T`? If yes should you, do it?
- Ja, man kann einen anderen Platzhalter einfügen, aber es ist nicht üblich. Üblicher ist: T für Typ und E für Element
- 
* Which benefits does this data structure have?
- Man kann diesen als Platzhalter als Klassentyp. Man läßt diesen Typ sozusagen offen und weist diesen dann bei der Befüllung des Array sozusagen erst zu. Auch bei Funktionen nutzbar. Man kann auch auf Methoden der Klasse zugreifen. Man kann mehrere Parameter eingeben -> noch mehr Variablen nutzbar.
* Which drawbacks does it have? Name a use case.
- Man sollte wissen, welcher Buchstabe für was steht. Nicht zu viele Platzhalter verwenden, da es nicht mehr übersichtlich ist.
---
> **NOTES:**
Write readable and good code. Do not repeate yourself use final,
static and access modifiers accordingly. Do not forget equals methods
for your own classes.
