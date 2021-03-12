# Projeto Integrado
Exercício de desenvolvimento de um sistema desktop de controle de projetos acadêmicos em Java.

## Descrição do Sistema
O trabalho consiste em desenvolver um sistema de controle de projetos acadêmicos. Nele
um usuário qualquer poderá criar projetos, associar a ele trabalhos de conclusão e artigos
científicos.
Para que seja possível cadastrar um novo projeto, antes é necessário cadastrar informações
sobre o responsável. Os dados do responsável são:

### RESPONSÁVEL
- Código (Obrigatório)
- Nome (Obrigatório)
- E-mail (Opcional)

Depois que os responsáveis forem cadastrados, um projeto poderá ser criado, ele deve
armazenar os seguintes dados:

### PROJETO

- Código (Obrigatório)
- Código do responsável (Obrigatório)
- Data de início e fim (Obrigatório)
- Situação atual (Em andamento, Cancelado ou Finalizado) – Padrão em Andamento

Cada projeto pode possuir associado a ele nenhum ou vários trabalhos de conclusão de curso
(TCC) e um TCC pode esta associado a APENAS um projeto.

### TCC
- Código (Obrigatório)
- Código do Projeto (Opcional)
- Título (Obrigatório)
- Nome do autor (Obrigatório)
- Situação (Em desenvolvimento, Defendido ou Abandonado) – Padrão em Desenvolvimento

Cada projeto pode possuir associado a ele nenhum ou vários artigos e um artigo pode estar
associado a APENAS um projeto.

### ARTIGO
- Código (Obrigatório)
- Código do Projeto (Opcional)
- Título (Obrigatório)
- Natureza (Resumo ou Completo) – Padrão Resumo
- Autor principal (Obrigatório)
- E-mail do autor principal (Obrigatório)

Além disso, cada artigo pode possuir NENHUM ou VÁRIOS coautores, e cada coautor
DEVE estar associado a um artigo.

### COAUTOR
- Código (Obrigatório)
- Código do Artigo (Obrigatório)
- Nome (Obrigatório)
- E-mail (Obrigatório)
Outras Considerações Sobre o Funcionamento do Sistema
- Deve existir tabelas SEPARADAS para exibir todos os projetos, responsáveis, tccs, artigos e
coautores cadastrados.
- Ao clicar duas vezes em um item de uma tabela deve ser aberta uma nova janela mostrando
detalhadamente os dados do item escolhido.
- Os registros das tabelas podem ser alterados.
- Os itens das tabelas pode ser apagados.
- Quando for exibido o detalhamento de um projeto, devem ser exibidas tabelas que mostrem todos
os TCCs e Artigos associados ao projeto.
- Um registro não pode ser salvo SOMENTE quando todos os campos obrigatórios estiverem
preenchidos.
- Antes de apagar um item da tabela exiba uma MENSAGEM DE CONFIRMAÇÃO.
