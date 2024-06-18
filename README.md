# TRABALHO-LAB.-COMPUTA-O
README
Este projeto implementa um sistema básico de uma biblioteca com classes em JavaScript, permitindo gerenciar livros, membros e empréstimos. Abaixo estão detalhadas as classes principais e suas funcionalidades.

Classes
Livro

Representa um livro com atributos como título, autor, ano de publicação, gênero, ISBN e disponibilidade.
Métodos:
toString(): Retorna uma representação em string do livro contendo título, autor e ISBN.
pegar(): Marca o livro como indisponível quando emprestado.
devolver(): Marca o livro como disponível quando devolvido.
Membro

Representa um membro da biblioteca com informações como nome, ID, data de nascimento, endereço e lista de livros emprestados.
Métodos:
toString(): Retorna uma representação em string do membro contendo nome e ID.
pegarLivro(livro): Permite que o membro pegue um livro emprestado, respeitando o limite de até 3 livros por vez.
devolverLivro(livro): Permite que o membro devolva um livro emprestado.
Emprestimo

Representa um empréstimo de um livro por um membro da biblioteca, com informações como o livro emprestado, o membro que o pegou, datas de empréstimo, vencimento e devolução.
Métodos:
toString(): Retorna uma representação em string do empréstimo contendo informações básicas.
atrasado(): Verifica se o empréstimo está atrasado com base na data de vencimento.
Biblioteca

Classe principal que gerencia os livros, membros e empréstimos na biblioteca.
Métodos:
adicionarLivro(livro): Adiciona um livro à coleção da biblioteca.
removerLivro(livro): Remove um livro da coleção da biblioteca.
Utilização
Para usar este código:

Incluir no seu projeto:

Copie o código das classes Livro, Membro, Emprestimo e Biblioteca para seu ambiente de desenvolvimento.
Exemplo de uso:

javascript
Copiar código
// Exemplo de uso das classes
let livro1 = new Livro("Aprendendo JavaScript", "João da Silva", 2020, "Tecnologia", "1234567890");
let membro1 = new Membro("Maria Souza", 001, new Date(1990, 5, 15), "Rua das Flores, 123");

let biblioteca = new Biblioteca();
biblioteca.adicionarLivro(livro1);
membro1.pegarLivro(livro1);
console.log(membro1.livrosEmprestados);
Contribuição
Contribuições são bem-vindas. Para mudanças significativas, por favor abra uma issue primeiro para discutir o que você gostaria de mudar.
