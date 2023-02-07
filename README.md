# Projeto_Individual_M4


## Sobre o projeto
A proposta do projeto foi criar um modelo de banco de dados fictício para o sistema de acompanhamento da Resilia.

Nessa modelagem temos 3 entidades já existentes ('cursos', 'turmas' e 'alunos'). Além de planejar e elaborador o banco de dados.
Foi nos proposto responder algumas perguntas feitas pelo cliente do banco de dados:

### 1 - Existem outras entidades além dessas três?

Sim. Podemos atribuir outras entidades na modelagem como a Instituição Resilia/Senac; uma entidade associativa como matricula, para relacionar cursos aos alunos.

### 2 - Quais são os principais campos e tipos?

Principais campos: 'ID', 'cpf', 'nome', 'telefone', 'nascimento', 'email';

Principais tipos: 'VARCHAR' e 'INT'.

### 3 - Como essas entidades estão relacionadas?

A 'instituicao' possui 'funcionarios', que por sua vez estão atrelados às 'turmas', que possuem 'cursos' que por fim têm 'alunos'.

Os 'funcionarios' possuem uma (FK) com a (PK) 'instituicao_cpnj' criando assim um vínculo entre as entidades.


Os 'cursos' também possuem uma (FK) com a (PK) 'instituicao_cpnj' para realizar a conexão.

As 'turmas' estão conectadas aos 'cursos' pela (FK) com a (PK) 'curso_id' e também aos 'alunos' com a (FK) da (PK) 'aluno_cpf'

Entidades
'instituicao' -
'funcionarios' -
'cursos' -
'turmas' -
'alunos' -
'docentes' -
'matrícula'

![Modelagem_projeto_Ind_M4](https://user-images.githubusercontent.com/113534772/217143494-20bfee40-501f-4f68-b567-02c440857052.jpg)
