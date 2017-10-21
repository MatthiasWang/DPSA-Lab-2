The `DB` and `DBTable` classes remain the same, and we added an abstract class `DBStorage` to the project. The `DB` class inherits `DBStorage`, which works as a concrete class, and we created a `DBDecorator` inheriting the `DBStorage` as a root class of decorators. `DBDecorator` also have an instance field of `DBStorage`, which stores the `DB`, and `DBDecorator` delegates its methods. `ConsoleLoggingDBDecorator` and `FileLoggingDBDecorator` works properly to record in console or file. 