// Función para determinar si una palabra o frase es un palíndromo
function esPalindromo(frase) {
    // Eliminar espacios y convertir la frase a minúsculas
    const fraseLimpia = frase.replace(/\s+/g, '').toLowerCase();

    // Invertir la frase limpia
    const fraseInvertida = fraseLimpia.split('').reverse().join('');

    // Comparar la frase original limpia con la invertida
    if (fraseLimpia === fraseInvertida) {
        console.log(`"${frase}" es un palíndromo.`);
    } else {
        console.log(`"${frase}" no es un palíndromo.`);
    }
}

// Ejemplo de uso
esPalindromo("Anita lava la tina");  // Ejemplo de palíndromo
esPalindromo("Hola mundo");  // Ejemplo de no palíndromo
