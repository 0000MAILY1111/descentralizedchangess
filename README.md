Trabajo Final: Creación de un Exchange Descentralizado Simple con Pools de Liquidez
Descripción del Proyecto:
Los estudiantes deben desplegar contratos inteligentes en la red de Scroll Sepolia (verificados y publicados) para implementar un exchange descentralizado simple que intercambie dos tokens ERC-20.

La solución debe permitir:

Añadir liquidez: El owner puede depositar pares de tokens en el pool para proporcionar liquidez.
Intercambiar tokens: Los usuarios pueden intercambiar uno de los tokens por el otro utilizando el pool de liquidez.
Retirar liquidez: El owner puede retirar sus participaciones en el pool.
Requisitos:
Crear dos tokens ERC-20 simples: Los contrato de los tokens deben tener obligatoriamente los nombres TokenA y TokenB.
Implementar un contrato de exchange (denominado obligatoriamente SimpleDEX) que:
Mantenga un pool de liquidez para TokenA y TokenB.
Utilice la fórmula del producto constante (x+dx)(y-dy) = xy para calcular los precios de intercambio.
Permita añadir y retirar liquidez.
Permita intercambiar TokenA por TokenB y viceversa.
El contrato SimpleDEX debe contar obligatoriamente y sin modificación de la interface con las siguientes funciones:
constructor(address _tokenA, address _tokenB)
addLiquidity(uint256 amountA, uint256 amountB)
swapAforB(uint256 amountAIn)
swapBforA(uint256 amountBIn)
removeLiquidity(uint256 amountA, uint256 amountB)
getPrice(address _token)
Incluir los eventos que consideren convenientes.
Objetivos de Aprendizaje:
Comprender cómo funcionan los exchanges descentralizados y los pools de liquidez.
Practicar la creación de tokens ERC-20 en Solidity.
Aprender a implementar mecanismos de mercado automatizados simples.
Llamar a otros contratos inteligentes.
