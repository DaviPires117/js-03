<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Processamento de Frutas</title>
</head>
<body>

  <script>
    function processarFrutas(fruta1, fruta2, fruta3, fruta4, fruta5) {
      
      return listaFrutas;
    }

    
    const resultado = processarFrutas("  Maçã", "Banana", "Laranja", "  Melancia", "  Morango");
    
    
    console.log(resultado);

  
    document.write(`<pre>${resultado}</pre>`);
  </script>

</body>
</html>


function processarFrutas(fruta1, fruta2, fruta3, fruta4, fruta5) {
  
  const lenFruta1 = fruta1.length;
  const lenFruta2 = fruta2.length;
  const lenFruta3 = fruta3.length;
  const lenFruta4 = fruta4.length;
  const lenFruta5 = fruta5.length;

  
  const subFruta1 = fruta1.substring(0, 3);
  const subFruta2 = fruta2.substring(0, 3);
  const subFruta3 = fruta3.substring(0, 3);
  const subFruta4 = fruta4.substring(0, 3);
  const subFruta5 = fruta5.substring(0, 3);

  
  const trimFruta1 = fruta1.trim();
  const trimFruta2 = fruta2.trim();
  const trimFruta3 = fruta3.trim();
  const trimFruta4 = fruta4.trim();
  const trimFruta5 = fruta5.trim();

 
  const lowerFruta1 = trimFruta1.toLowerCase();
  const lowerFruta2 = trimFruta2.toLowerCase();
  const lowerFruta3 = trimFruta3.toLowerCase();
  const lowerFruta4 = trimFruta4.toLowerCase();
  const lowerFruta5 = trimFruta5.toLowerCase();

  
  const listaFrutas = `
    Fruta 1: ${lowerFruta1}
    Comprimento: ${lenFruta1}
    3 Primeiros Caracteres: ${subFruta1}

    Fruta 2: ${lowerFruta2}
    Comprimento: ${lenFruta2}
    3 Primeiros Caracteres: ${subFruta2}

    Fruta 3: ${lowerFruta3}
    Comprimento: ${lenFruta3}
    3 Primeiros Caracteres: ${subFruta3}

    Fruta 4: ${lowerFruta4}
    Comprimento: ${lenFruta4}
    3 Primeiros Caracteres: ${subFruta4}

    Fruta 5: ${lowerFruta5}
    Comprimento: ${lenFruta5}
    3 Primeiros Caracteres: ${subFruta5}
  `;

  return listaFrutas;
}


const resultado = processarFrutas("  Maçã", "Banana", "Laranja", "  Melancia", "  Morango");
console.log(resultado);
