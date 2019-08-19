## Teste Backend Nodejs
Somos uma startup que desenvolve soluções na área da saúde e por conta disso trabalhamos com muitos dados sensiveis, logo precisamos de uma arquitetura de software eficiente e robusta. Neste teste além da parte funcional iremos avaliar qualidade do código, performance e padrões de projeto.

## Desafio
Precisamos saber qual é a equipe médica que está responsável pela internação de um paciente em determinado leito, para isso teremos os seguintes campos: Leitos, pacientes, médico e enfermeiro(a)s.

Cada leito tem um paciente, um médico responsável e pode ter mais que um enfermeiro(a) em monitoramento. Desenvolva uma API REST que irá alimentar cada item e que seja capaz de vincular [ paciente x leito ], [ médico x leito ], [ enfermeiros x leito ].

## Tabelas
- Leitos (id, paciente, médico, enfermeiros)
- Paciente (id, nome, cpf)
- Médico (id, nome, crm)
- Enfermeiro (id, nome, coren)

## Critérios lógicos
- Leito não pode ser aberto sem escolher um usuário existente, médico e no mínimo um enfermeiro(a).
- Leito deve conter apenas um único médico e pode conter vários enfermeiro(a)s.

## Endpoints
- CRUD Paciente
- CRUD Medico
- CRUD Enfermeiros
- Vincular Paciente a um leito, informando o médico e enfermeiro(a)s
- Retornar leitos usados
- retornar todos os leitos onde o médico é responsável informado via CRM.
- retornar todos os leitos onde o enfermeiro(a) está trabalhando via COREN.

## Critérios técnicos
- Javascript ES6
- Typescript
- Nodejs
- Express
- Mongodb
- Docker (imagem para aplicação e outra para banco de dados)


## Entrega
A entrega do seu teste deve ser um reposótorio no github com readme de instruções para rodar a aplicação seguindo todos critétios técnicos e lógicos listados acima. Após termino basta abrir uma issue e postar link do repositório.

