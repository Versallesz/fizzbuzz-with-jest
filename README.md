# fizzbuzz-with-jest
resolving a practical programming test with js and jest for testing, and yes, in English

Ahora ante la pereza y poca asignación de tiempo por mi parte para realizar esta mini documentación, realizaré esta parte en español.

### Qué hacer para tener Jest
Al tener la carpeta creada de Fizzbuzz, nos dirigimos a la consola en la carpeta y ponemos lo siguiente: 
1. `npm init -y`
2. `npm i -D jest` Instalar librería jest en modo desarrollo.
3. `npx jest --init` Configurar jest.
	- `Would you like to use Jest when running "test" script in "package.json"? » (Y/n) y`
	- ` Would you like to use Typescript for the configuration file? » (y/N) n`
	- ` Choose the test environment that will be used for testing » - Use arrow-keys. Return to submit >   node // jsdom (browser-like)`  Node estará seleccionado, solo dar enter.
	- `Do you want Jest to add coverage reports? » (y/N) y `
	- ` Which provider should be used to instrument code for coverage? » - Use arrow-keys. Return to submit. > v8 // babel` Enter en v8
	-  ` Automatically clear mock calls and instances between every test? » (y/N) y`

#### Configurar para que corra los test automaticamente
En el package.json en la sección de `"scripts"` agregar debajo de`"test": "jest",` :
	`"test:watch": "jest --watchAll"`

Luego para correr esto poner en la terminal: `npm run test:watch`

Si no hay test, fallará, pero ya se pueden crear los archivos de fizzbuzz.js y fizzbuzz.test.js :) 

