                          TASK1  SUSTITUCION POR DESPLAZAMIENTO - CIFRADO CESAR
ANALISIS

1. Sanear el texto:
Poner todo en mayúsculas: Esto se hace para simplificar el proceso, ya que solo trabajaremos con las 26 letras del alfabeto mayúscula. De esta forma, evitamos tener que lidiar con minúsculas, tildes o diéresis.
Quitar signos y números: Los signos de puntuación, acentos y números no son parte del alfabeto que vamos a usar para el cifrado. Al eliminarlos, nos aseguramos de que solo trabajemos con las letras que nos interesan.

2. Convertir letras a números:
Para poder realizar cálculos matemáticos, necesitamos representar cada letra por un número. Lo más común es asignar un número del 0 al 25 a cada letra, empezando por la A como 0, la B como 1, y así sucesivamente hasta la Z como 25.

3. Aplicar la fórmula Ci = mi + k mod 26:
Ci: Representa la letra cifrada.
mi: Representa la letra original.
k: Es la clave, es decir, el número de posiciones que desplazamos cada letra en el alfabeto.
mod 26: Esta operación asegura que el resultado siempre esté entre 0 y 25, ya que solo tenemos 26 letras en el alfabeto.
Ejemplo:
Si queremos cifrar la letra "A" (que equivale a 0) con una clave de 3, aplicamos la fórmula:
Ci = 0 + 3 mod 26 = 3
El resultado es 3, que corresponde a la letra "D".

4. Romper el cifrado: Análisis de frecuencia
El análisis de frecuencia se basa en la idea de que cada letra del alfabeto aparece con una frecuencia determinada en un idioma. Por ejemplo, en español, la letra "E" es la más común.
Para romper un cifrado César, podemos:
Calcular la frecuencia de cada letra en el texto cifrado: Contamos cuántas veces aparece cada letra en el texto cifrado.

5. Comparar con la frecuencia esperada:
Comparamos las frecuencias obtenidas con las frecuencias esperadas para el idioma en el que está escrito el mensaje.

6. Probar diferentes claves: Probamos diferentes valores de "k" hasta encontrar el que hace que la frecuencia de las letras en el texto descifrado se parezca más a la frecuencia esperada.

7. Índice de coincidencia
El índice de coincidencia es una medida estadística que nos ayuda a estimar la longitud de la clave en cifrados más complejos. Se basa en comparar la frecuencia de las letras en diferentes partes del texto cifrado. Un valor alto del índice de coincidencia indica que es probable que esas partes estén cifradas con la misma clave.



PROMPT PARA HALLAR CLAVE (SCRIPT_SOLUCION_TK1)
1.	Limpie un texto: Convierta a mayúsculas, elimine signos de puntuación, números y espacios del siguiente texto cifrado: 'NOYZU XEOYV ATIZA GZKJC OZNIU JKYZN KENGB KJKIO JKJZN KUAZI USKYU LHGZZ RKYGT JRKJZ UZNKJ KGZNY ULQOT MYGTJ WAKKT YONGB KZNKX KLUXK HKKTG HRKZU IGRRA VUTYZ UXOKY ULVUR OZOIG ROTZX OMAKG TJZGR KYULR OLKGT JJKGZ NZUOR RAYZX GZKZN KQKEZ AXTOT MVUOT ZYOTZ NKKBU RAZOU TGXEJ KBKRU VSKTZ ULIUJ KYZNK NOYZU XEULI UJKYO YYUOT UXJOT GZKRE XOINZ NGZON GBKHK KTLUX IKJZU RKGBK UAZSG TELGY IOTGZ OTMYZ UXOKY CNOIN OTZAX TSKGT YZNGZ SEGII UATZO YTUZJ KLOTO ZOBKO LEUAC UARJR OQKZU LOTJU AZSUX KGHUA ZEUAX LGBUX OZKZG RKUXE UAXLG BUXOZ KIUJK HXKGQ KXZNK TOCUA RJXKL KXEUA ZUZNK ROYZU LLAXZ NKXXK GJOTM CNOIN YNUAR JNKRV ZNUYK XKGJK XYCNU CUARJ ROQKZ UYZAJ EZNKY AHPKI ZOTSU XKJKZ GOR'.
2.	Convierta a números: Asigne a cada letra mayúscula un número del 0 al 25 (A=0, B=1, ...).
3.	Descifre por desplazamiento: Utilice un algoritmo de fuerza bruta para probar todos los posibles desplazamientos (del 1 al 25) en el cifrado por sustitución de desplazamiento.
4.	Analice la frecuencia de letras: Para cada desplazamiento, compare la frecuencia de las letras resultantes con la frecuencia esperada en el idioma inglés (o el idioma correspondiente).
5.	Identifique el mejor desplazamiento: Seleccione el desplazamiento que produzca un texto descifrado con la distribución de frecuencias más cercana a la del idioma natural."

PROMPT PARA ORDENAR TEXTO EN BLOQUE 5 CARACTERES (SCRIPT_SOLUCION_2_TK1)
script python que separe en bloque de 5 caracteres por espacio en blanco entre ellos al 
siguiente texto
HISTORYISPUNCTUATEDWITHCODESTHEYHAVEDECIDEDTHEOUTCOMESOFBATTLESANDLEDTOTHEDEATHSOFKINGSANDQUEENSIHAVETHEREFOREBEENABLETOCALLUPONSTORIESOFPOLITICALINTRIGUEANDTALESOFLIFEANDDEATHTOILLUSTRATETHEKEYTURNINGPOINTSINTHEEVOLUTIONARYDEVELOPMENTOFCODESTHEHISTORYOFCODESISSOINORDINATELYRICHTHATIHAVEBEENFORCEDTOLEAVEOUTMANYFASCINATINGSTORIESWHICHINTURNMEANSTHATMYACCOUNTISNOTDEFINITIVEIFYOUWOULDLIKETOFINDOUTMOREABOUTYOURFAVORITETALEORYOURFAVORITECODEBREAKERTHENIWOULDREFERYOUTOTHELISTOFFURTHERREADINGWHICHSHOULDHELPTHOSEREADERSWHOWOULDLIKETOSTUDYTHESUBJECTINMOREDETAIL


