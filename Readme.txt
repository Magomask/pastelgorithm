-- El resultado de la "torta" es una combinatoria del siguiente modo
-- A = cantidad de posiciones fila {a11,b11,c11,a21,b21,c21,a31,b31,c31} 
-- B = cantidad de posiciones columna {a11,b12,c12,a12,b12,c12,a13,b13,c13}

-- filas SIN masitas = (A!*A)^3
-- filas CON masitas = (A!*A)^3 
-- 	FILAS TOTALES => (A!*A)^3 + (A!*A)^3   =   (A!*A)^3 * 2

-- columnas SIN masitas = (B!*B)^3
-- columnas CON masitas = (B!*B)^3 
-- 	COLUMNAS TOTALES => (B!*B)^3 + (B!*B)^3   =   (B!*B)^3 * 2

-- Como A = B
----------------
 (A!*A)^3 * 4
---------------- 

 -->> RESULTADO
  
   (3!*3)^3*4 = 23328

--Explicación
-- 3! = indica la cantidad de posiciones que puede tomar cada ingrediente por 1 fila
-- *3 = indica la cantidad de posiciones que puede tomar cada ingrediente para todas las filas
-- ^3 = realiza la combinatoria entre la posición de cada ingrediente vs los otros 2
-- *4 = 5832 combinaciones horizontales con los ingredientes + 5832 combinaciones verticales con los ingredientes + 5832 combinaciones horizontales con 2 ingredientes y una masita + 5832 combinaciones verticales con 2 ingredientes y una masita