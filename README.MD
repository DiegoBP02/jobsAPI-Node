Projeto feito através do curso do John Smilga de Node. Possui as seguintes funcionalidades:
- Possui um sistema de login/registro que permite o usuário acessar as funcionalides do projeto
- Caso o login tenha sido realizado, o usuário consegue:
- Criar vagas de trabalho(Create Job),
- obter todas as vagas(Get all Jobs),
- obter uma vaga específica(Get Single Job),
- atualizar as informações de uma vaga específica(Update Job) e 
- deletar uma vaga específica(Delete Job).
- Projeto utiliza o banco de dados MongoDB através da biblioteca mongoose
- Senha criptografada com o bcryptjs para assegurar a segurança do usuário
- Quando o usuário se loga e passa na autenticação, um token é gerado através da biblioteca jsonwebtoken, que autoriza o usuário acessar as funcionalidades do projeto
- Manipulação de erros para erros de validação do mongoose, de emails duplicados e cast errors
- Uso das bibliotecas helmet, cors e xss-clean para a segurança do projeto
- Uso da biblioteca express-rate-limit para limitar o número de acessos por um usuário
- O arquivo json é documentado através da ferramenta APIMatic e editado através do Swagger Editor
- Projeto implantado na nuvem através do sistema de nuvem Render



In order to run the project, in the root create .env with these two variables, with your own values.

MONGO_URI
JWT_SECRET

After that run this command

npm install && npm start
