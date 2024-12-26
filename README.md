# zatten-test

- Deve ser criado um sistema com autenticação usando o clerk (https://clerk.com/), esse sistema deve permitir login e cadastro com email e senha e com alguma autenticação de terceiro, ex: google.
- No sistema tábem deve ter um dashboard com a listagem de chats já existentes, esses chats devem ser do usuário autenticado.
- Os chats devem persistir no banco de dados supabase
- Deve ser possível criar chats novos
- Os chats devem ser chats com a IA da open AI usando assistentes (https://platform.openai.com/docs/assistants/overview)
- Deve ser possível criar um chat e conversar com o assistente, ou selecionar um chat já criado anteriormente e continuar a conversa
- Basicamente a aplicação é como um chatGPT
- Você pode criar o layout da sua preferência
- A aplicação deve expor um endpoint (api) para criar um chat novo, passando id ou email do usuário (para fazer o vínculo), e um título para ser mostrado na listagem. Ao criar um novo chat através da request (voce pode usar o insomnia ou postman para testar isso), deve ser criado a thread e salvar no banco, esse chat deve ser mostrado ao vivo na tela de listagem de chats, consulte a documentação do supabase realtime (https://supabase.com/docs/guides/realtime)

Tecnologias obrigatórias: Next, shadcn ui, supabase
Permitido e incentivado o uso de ferramentas de IA para a criacão do sistema. ex: cursor, v0, lovable, bolt.new etc.

Opcional:
Seria interessante ter um script de migração de usuário. por exemplo, usar o array de usuário abaixo para inserir todos os usuários no clerk e pedir a criação de senha ou recuperação, ou algo do tipo, mas mantendo o id do usuário.

[
  {
    "id": "123456789",
    "name": "Fulano",
    "email": "fulano@zatten.com",
    "password": "kd98e1289jdbaahjdgajsdajd90281903shdajkasdhjagsdhajsdgashjd",
  },
  {
    "id": "985678253",
    "name": "Siclano",
    "email": "siclano@zatten.com",
    "password": "kd98e1289jdbaahjdgajsdajd90281903shdajkasdhjagsdhajsdgashjd",
  },
  {
    "id": "888765198",
    "name": "Joaquim",
    "email": "joaquim@zatten.com",
    "password": "kd98e1289jdbaahjdgajsdajd90281903shdajkasdhjagsdhajsdgashjd",
  },
  {
    "id": "907243748",
    "name": "aquele cara",
    "email": "aquele_cara@zatten.com",
    "password": "kd98e1289jdbaahjdgajsdajd90281903shdajkasdhjagsdhajsdgashjd",
  },
]
