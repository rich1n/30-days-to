### Ejemplo de un código escrito en Solidity con sus definiciones


    pragma solidity ^0.4.0;

    contract SimpleStorage {
      uint storedData;

      function set(uint x) {
          storedData = x;
      }

      function get() constant returns (uint) {
          return storedData;
      }
    }


Primera línea
Dice que el código fuente se ha escrito en la versión 0.4.0 de Solidity o en otra superior totalmente compatible (cualquiera anterior a la 0.5.0).
Esto es para garantizar que el contrato no se va a comportar de una forma diferente con una versión más nueva del compilador.
La palabra reservada pragma es llamada de esa manera porque, en general, los “pragmas” son instrucciones para el compilador que indican como este debe operar con el código fuente.

