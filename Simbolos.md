# Símbolos

### Definición:
    • Tipo de dato primitivo como string, number, boolean, null y undefined
    • Valores únicos e immutables, es decir, la función Symbol() permite obtener identificadores únicos y diferentes a los ya creados y a los por crear
    • Se les puede agregar una descripción que facilite su identificación (recomendado)
    
### Otras características:
    • Se debe utilizar Objeto.getOwnPropertySymbols() para poder enumerar las propiedades de un objeto cuyas claves son Symbol
    • No sufren “casting ” de tipos (no se convierten implícitamente en otro tipo como string)
    
### Usos:
    • Los valores únicos que se producen con Symbol() pueden ser utilizados como claves (keys) de de los objetos y así poder crear nuevas propiedades sin que éstas entren en conflicto con las existentes. Ésto es particularmente útil cuando se habla de objetos “grandes” como el objeto global Wnindow
    • Evita la sobreescritura de propiedades y métodos ya existentes
    • Como las propiedades con claves Symbol() no son enumeradas por Objeto.keys u Objeto.getOwnPropertyNames, pueden utilizarse para definir propiedades privadas
    • Pueden utilizarse para definir una lista de constantes, ejemplo una lista de descripciones de errores

### Propiedades y métodos:

| **Propiedad** | **Descripción** | **Ejemplo** |
| ------------- | ------------- | ------------- |
| Symbol.length  | Es 0 para todos los símbolos  |   |
| **Método**  |  |   |
| Symbol.for(key)  | Devuelve el símbolo creado con la clave dada. Si no existe, un nuevo símbolo se crea |   |
| Symbol.keyFor(sym)  | Devuelve la clave del símbolo dado |   |

### Símbolos más conocidos:

| **Symbol** | **Descripción** |
| ------------- | ------------- |
| Symbol.hasInstance  | Método usado por instanceof para determinar la herencia de un objeto |
| Symbol.iterator  | Método que devuelve un iterador |
| Symbol.match  | Método usado por String.prototype.match() para comparar strings |
| Symbol.replace  | Método usado por String.prototype.replace() para reemplazar substrings |
| Symbol.search  | Método usado por String.prototype.search() para buscar substrings |
| Symbol.species  | Constructor utilizado para crear objetos derivados |
| Symbol.split  | Método usado por String.prototype.split() para dividir strings |
| Symbol.toPrimitive  | Método que devuelve una representación del valor primitivo de un objeto |
| Symbol.toStringTag  | Un string utilizado por Object.prototype.toString() para crear una descripción de objeto |
| Symbol.unscopables  | Un objeto cuyas propiedades son los nombres de las propiedades del objeto que no deben incluirse en una declaración with |













