# Gerenciador-de-tarefas
Um simples gerenciador de tarefas para o seu dia a dia 😁.



# Lista de Tarefas 📌

## Descrição

Esta aplicação é uma lista de tarefas simples, que permite adicionar, marcar e excluir tarefas. 

## Estrutura do Código

### `index.html`

Define o layout da aplicação de lista de tarefas. Contém um cabeçalho com o título, um campo de entrada para novas tarefas, um botão de adição, e um contêiner `<ul>` que exibirá as tarefas adicionadas.

### Estilos (`styles.css`)

Os estilos são definidos para tornar a aplicação esteticamente agradável e responsiva. Utiliza a fonte "Acme" para um visual claro, ajusta o layout dos elementos, e trata interações como `:hover`.

### `script.js`

Contém a classe `Todo_Class` e a lógica associada para controle da lista de tarefas, permitindo adicionar novas tarefas, marcar tarefas como feitas/não feitas e excluir tarefas. A lista de tarefas é mantida em um array `todoObjectList`.

## Funções

### `constructor(item)`

Inicializa uma instância da classe com um elemento `ul`, onde as tarefas são exibidas.

### `add()`

Adiciona uma nova tarefa à lista. Verifica se o campo de entrada não está vazio e adiciona o objeto da tarefa ao `todoObjectList`. Em seguida, chama `display()` para atualizar a exibição da lista.

### `done_undone(x)`

Marca uma tarefa como feita ou não feita, alterando a propriedade `isDone` do objeto da tarefa. Atualiza a exibição chamando `display()`.

### `deleteElement(z)`

Remove uma tarefa do `todoObjectList` com base em seu `id`. Atualiza a exibição chamando `display()`.

### `display()`

Esvazia o elemento `ul` e adiciona cada tarefa do `todoObjectList` como um elemento `li`. Adiciona um ouvinte de evento aos ícones de exclusão e linhas para lidar com a marcação e exclusão de tarefas.

## Interação do Usuário

Os usuários podem interagir com a aplicação de várias maneiras:

- Digitando uma tarefa e clicando no botão de adição ou pressionando "Enter".
- Clicando em uma tarefa para marcá-la como feita ou não feita.
- Clicando no ícone da lixeira para excluir uma tarefa.

## Recursos Externos

- **Font Awesome**: Ícones para o botão de adição e exclusão de tarefas.
- **Google Fonts**: Para a fonte "Acme" usada em todo o aplicativo.
