<script setup>
const miVariable = 'Mi objeto ';
function miFuncion() {
  return 7;
}

const frases = [
  {
    frase:
      'La más bella palabra en labios de un hombre es la palabra madre, y la llamada más dulce: madre mía.',
    autor: 'Khalil Gibran (1883-1931) Ensayista, novelista y poeta libanés.',
    tema: 'madres',
  },
  {
    frase: 'Hay un solo niño bello en el mundo y cada madre lo tiene.',
    autor: 'José Martí (1853-1895) Político y escritor cubano.',
    tema: 'madres',
  },
  {
    frase:
      'A una madre se la quiere siempre con igual cariño y a cualquier edad se es niño cuando una madre se muere.',
    autor: 'José María Pemán (1898-1981) Escritor español.',
    tema: 'madres',
  },
  {
    frase: 'El porvenir de un hijo es siempre obra de su madre.',
    autor: 'Napoleón I (1769-1821) Napoleón Bonaparte. Emperador francés.',
    tema: 'madres',
  },
  {
    frase:
      'Jamás en la vida encontraréis ternura mejor y más desinteresada que la de vuestra madre.',
    autor: 'Honoré de Balzac (1799-1850) Escritor francés.',
    tema: 'madres',
  },
  {
    frase: 'Las madres perdonan siempre: han venido al mundo para eso.',
    autor: 'Alejandro Dumas (1802-1870) Escritor francés.',
    tema: 'madres',
  },
  {
    frase: 'La mano que mece la cuna rige el mundo.',
    autor: 'Peter de Vries (1910-1993) Editor y novelista estadounidense.',
    tema: 'madres',
  },
  {
    frase: 'Quien quiere a su madre no puede ser malo.',
    autor: 'Alfred de Musset (1810-1857) Poeta francés.',
    tema: 'madres ',
  },
  {
    frase:
      'Todo lo que soy o espero ser se lo debo a la angelical solicitud de mi madre.',
    autor: 'Abraham Lincoln (1808-1865) Político estadounidense.',
    tema: 'madres',
  },
  {
    frase: 'La mano que mece la cuna es la mano que gobierna el mundo.',
    autor: 'William Ross Wallace (1819-1892) Poeta estadounidense.',
    tema: 'madres',
  },

  {
    frase:
      'El corazón de una madre es un abismo en el fondo del cual siempre hay un perdón.',
    autor: 'Honoré de Balzac (1799-1850) Escritor francés.',
    tema: 'madres',
  },
  {
    frase:
      '¿Cómo no amarte, madre, si me enseñaste a hablar tu lengua? ¿Si soy viento nacido de tu roca?',
    autor: 'Gonzalo Rojas (1916-2011) Profesor y periodista chileno.',
    tema: 'madres',
  },
  {
    frase:
      'Muchas maravillas hay en el universo; pero la obra maestra de la creación es el corazón materno.',
    autor: 'Ernest Bersot (1816-1880) Filósofo francés.',
    tema: 'madres',
  },
];

</script>

<template>
  <h1>Frases celebres</h1>
  <!-- OJO se usan comillas dobles. Recorre el objeto o la matriz. por cada obejeto que ya existe lo recorre
          Repite el bucle 13 frases porque son las frases que hay. 'frase' es una variable. Si yo no quiero todo el objeto sino 
          solo una partes se puede desestructurar con {}
          Puedo quitar 'tema y puedo poner autor antes, no importa el orden' 
        Si yo quiero cambiar 'frase por otro nombre puedo poner frase:cita'-->
  <ul>
    <li v-for="( frase, index ) in frases">
      <span>({{ index + 1 }}){{ frase.frase }}</span>
      <blockquote> - {{ frase.autor }}</blockquote>
    </li>
  </ul>
</template>

