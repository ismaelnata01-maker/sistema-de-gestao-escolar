# Sistema de Gestão Escolar

## Sistema para gerenciar funcionarios, alunos, cursos e matrículas

1. Quem utilizará o sistema (usuários)?
    - Funcionários

2. Quais os tipos de usuários e o que cada tipo consegue fazer?
       - Colaboradores: Cadastrar alunos, cadastrar cursos, editar dados dos alunos,
    editar dados dos cursos, excluir alunos, excluir cursos, listar alunos, listar cursos,
    matricular alunos nos cursos, desmatricular alunos dos cursos e atualizar os próprios dados.
       - Admin: Todas as funções acima, mais: cadastrar outros funcionários, listar outros funcionários,
    editar dados dos outros funcionários e excluir outros funcionários.

3. Quais informações iremos armazenar?
       - Funcionários: Nome, email, cargo, data de nascimento, cpf, senha,
    telefone, endereço.
       - Alunos: Matrícula, cpf, nome, data de nascimento, email, telefone, endereço.
       - Cursos: Descrição, carga horária, nome.
       - Matrículas: Quais alunos estão cadastrados em quais cursos

4. Quais regras ou restrições são necessárias?
       - Apenas funcionários admin podem criar/deletar outros funcionários.
       - Funcionários colaboradores não podem editar dados de outros funcionários.
       - CPF não pode repetir, email não pode repetir.
       - Nome, email, cargo, CPF, senha, carga horária, matrícula são dados obrigatórios.
       - Um aluno não pode ser matriculado 2 ou mais vezes no mesmo curso.
       - O sistema deve validar as informações.

## PROBLEMA:
 - Esse sistema é direcionado a funcionários de escolas
 - Permite cadastrar, editar, listar e deletar alunos, cursos, matrículas e funcionários

## MODELO DE NEGÓCIO:
  ![Business Model Canvas](./Captura%20de%20tela%202026-08-25%20170410.png)

## REQUISITOS:
1. Requisitos Funcionais:
  - Cadastrar alunos
  - Cadastrar funcionários
  - Cadastrar cursos
  - Listar alunos
  - Listar cursos
  - Listar funcionários
  - Mostrar os dados do aluno
  - Mostrar os dados dos funcionários
  - Mostrar os dados do curso
  - Realizar as matículas
  - Editar os dados do aluno
  - Editar os dados do funcionário
  - Editar os dados do curso
  - Excluir os alunos
  - Excluir os funcionários
  - Excluir os cursos
  - Excluir as matrículas

2. Requisitos não Funcionais:
  - Autenticação
  - Interface com navegação padronizada e consistente entre as telas
  - Interface responsiva e adaptativa à diversas resoluções de tela e dispositivos diferentes, como computador, celular e tablet
  - Interface deve ser compatível com os principais navegadores web
  - Criptografar as senhas antes de salvá-las no banco de dados

## ATIVIDADE:

Funcionais:

- ter lista de alunos que foram excluidos
- ter lista de funcionarios que foram excluidos
- ter lista de cursos que foram excluidos
- ter sistema de recuperação de alunos que foram excluidos
- ter sistema de recuperação de funcionarios que foram excluidos
- ter sistema de recuperação de cursos que foram excluidos
- ter sistema de recuperação de matrículas que foram excluidas

Não funcionais:

- senha ter mais de 8 caracteres
- senha ter letra maiuscula
- senha ter letra minuscula
- senha ter caractere especial
- não pode copiar senha
- não pode colar senha
- o funcionario não pode trocar suas informações em um intervalo de 30 dias desde a ultima alteração
- o aluno não pode trocar suas informações em um intervalo de 30 dias desde a ultima alteração
- o admin não pode trocar as informações de um curso em um intervalo de 30 dias desde a ultima alteração
- o admin não pode trocar as informações de um funcionário em um intervalo de 30 dias desde a ultima alteração
- o aluno só pode trocar de email com uma confirmação de uma mensagem de alerta enviada ao outro email
- o funcionario só pode trocar de email com uma confirmação de uma mensagem de alerta enviada ao outro email
- o aluno não pode trocar de CPF
- o profissional não pode trocar de CPF
- o aluno não pode alterar a data de nascimento
- o profissional não pode alterar a data de nascimento
- o Adimin não pode alterar as informações de um aluno
- o aluno não pode alterar as informações do profissional
- o aluno não pode alterar as informações do admin
- o profissional não pode alterar as informações do aluno
- o profissional não pode alterar as informações do admin
- alunos excluidos não tem mais acesso ao sistema
- profissionais excluidos não tem mais acesso ao sistema