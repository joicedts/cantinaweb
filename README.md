## Universidade do Estado da Bahia
#### Linguagens de Programação III
**Profª: Ana Patrícia Fontes Magalhães Mascarenhas**
#### Trabalho 2015.2

[![Cantina band 9 hours 59 minutes 59 seconds](http://img.youtube.com/vi/FWO5Ai_a80M/0.jpg)](https://www.youtube.com/watch?v=FWO5Ai_a80M)

### Orientações

**A atividade deve ser desenvolvida em grupos de no máximo 3 pessoas**

Para o cenário descrito a seguir  

**Primeira Parte (Data de Entrega: 15/03/2016):**  
* Construir a camada de Interface para o site com todas as opções de tela (1.0), navegação e validações em javaScript  (1.0). 
* Construa o processamento de uma página usando Servlet (1.0)
* Construa o processamento de uma página usando JSP (1.0)

**Segunda Parte (Data de Entrega: 10 e 13/05)**
* Construir os beans necessários (2.0)
* Construir os servlets de controle (2.0)
* Construir o banco e a camada de banco (1.0)
* Construir os DAOs (1.0)

### Descrição do cenário para a atividade

Considere um sistema web para cantinas de escolas que funciona da seguinte maneira:  

O sistema será utilizado por três tipos de usuários: funcionários, Responsáveis (ex. pai) e alunos.  
Quando um cliente qualquer acessa o sistema ele visualiza uma página inicial com algumas informações gerais da empresa e uma opção de login. Feito o login, a depender do tipo do usuário ele é direcionado para uma página com suas opções de acesso.  
Funcionários podem manter produtos, cadastrar pais, consultar o saldo dos alunos.  
Responsáveis podem cadastrar alunos, depositar crédito para um aluno, consultar saldo de um aluno, bloquear consumo de aluno e consultar consumo de aluno.  
Alunos podem comprar e consultar saldo.  
Quando o sistema é instalado em uma escola, é feito um cadastro da escola e de pelo menos um funcionário que ficará responsável pelo sistema.  
A seguir é detalhada cada uma das funcionalidades que devem existir no sistema para o funcionário: 
* Iniciando o sistema  
    * Apresentação de informações gerais do sistema (estática) e da escola (dinâmica) e opção de login. As informações gerais são logo e nome do sistema, objetivo do sistema, vantagens do sistema. As informações das escolas são nome da escola, endereço, telefone e email.
* Login
    * Solicitar login e senha e validar. 
* Manter produtos (incluir, alterar, bloquear, consultar, desbloquear)
    * Produtos podem ser comida ou bebida
    * Comidas devem ser cadastradas com código, nome, ingredientes e preço;
    * Bebidas devem ser cadastradas com código, nome, fornecedor e preço.
    * Todos os campos são obrigatórios.
* Manter Responsável
    * Todo responsável deve ser cadastrado com cpf, nome, telefone, email
    * Deve ser cadastrado também um login e senha para cada responsável
* Consultar Saldo de aluno
    * Nesta opção é informada a matricula do aluno e o sistema deverá trazer o valor em Real que o aluno possui de saldo na sua conta. Somente o próprio aluno, o responsável ou o funcionário poderá consultar o dado do aluno.
* Manter Aluno (incluir / alterar/ bloquear/consultar/desbloquear)
    * Os dados do aluno são: matricula, turma, turno, nome
* Depositar crédito
    * Nesta opção o responsável seleciona o aluno desejado e informa o valor do crédito. Este valor é adicionado no saldo do aluno.
* Bloquear consumo do aluno
    * Nesta opção é informada a matricula do aluno desejado e selecionados os produtos a serem bloqueados. Somente o responsável pode bloquear o consumo dos seus alunos.
* Consultar consumo do aluno
    * Nesta opção é informada a matricula do aluno desejado e o período desejado do consumo. O sistema deve listar por data todos os produtos consumidos pelo aluno. Somente o responsável pode consultar o consumo dos seus alunos.
* Comprar
    * Aluno escolhe os produtos desejados e conclui a compra. O sistema deve registrar a compra (data, produto) e abater do saldo do aluno o valor da compra.
