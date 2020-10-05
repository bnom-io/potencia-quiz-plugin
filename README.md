## Instalación del componente

El componente no se encuentra publicado como un paquete de npm, se encuentra disponible en un repositorio. Sin embargo, para instalarlo se utiliza el mismo método o comando, como cualquier paquete de npm.

El paquete se encuentra en el repositorio https://github.com/bnom-io/potencia-quiz-plugin y se instala a través del siguiente comando.

```bash
npm install --save https://github.com/bnom-io/potencia-quiz-plugin
```

## Utilizar componente

Para utilizar el componente primero se tiene que importar a través de la siguiente sentencia, como cualquier otro módulo de React.

```JavaScript
import Quiz from 'potencia-quiz';
```

## Componente Quiz

El componente `Quiz` únicamente recibe un parámetro llamado `id`, que debe contener la ruta correspondiente para encontrar su contenido en formato JSON.

```JSX
function showQuiz({discover_questions}) {
  console.log(discover_questions);
  # Imprime: /salon/176/lesson/37/some.json 
  return <Quiz id={discover_questions} />;
}
```
