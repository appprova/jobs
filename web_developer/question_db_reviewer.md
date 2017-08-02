# Desafio Técnico

### Descrição:

Você deverá implementar uma plataforma para o cadastro de questões.
Usuários comuns podem cadastrar e visualizar as suas questões, e usuários administradores poderão revisar e visualizar questões de todos os usuários;

---
- Ao se cadastrar, um novo usuário poderá criar questões, e também visualizar as questões já cadastradas por ele.

- Para criar uma questão, será necessário preencher os seguintes campos:
  - Conteúdo
  - Fonte
  - Ano
  - Alternativas

  onde, uma questão deverá ter 5 alternativas, com os seguintes campos:
    - Conteúdo
    - ID da questão
    - Correta

*obs:* todos os campos são obrigatórios

- Após salvar uma questão, ela automaticamente deverá ser marcada como "pendente";

- O status da questão será mostrado na página de visualizar questões do usuário (os possíveis status da questão são: "pendente", "aprovada", "reprovada").

- Se alguma questão estiver "reprovada", o usuário poderá editá-la, com base no comentário feito pelo administrador e submeter novamente. Nesse ponto o status da questão volta para "pendente".

---
- O usuário administrador deverá ser cadastrado separadamente (não necessariamente via browser).
- O administrador poderá visualizar as questões de todos os usuários, separadas em: questões pendentes, questões aprovadas e questões reprovadas.
- A visualização das questões deve identificar qual usuário foi o autor de cada questão.
- Ao visualizar as questões pendentes, um administrador pode abrir uma questão invidualmente para fazer a revisão da mesma.
- Se a questão for aprovada, ela é marcada como "aprovada".
- Se a questão for "reprovada", o administrador deve fornecer um comentário explicando os motivos da reprovação.

---
**Bonus:**
*Como o administrador poderá fazer várias revisões de uma mesma questão, ter o histórico dessas revisões é um diferencial.*

---
### Resultado esperado:

- Além dos requisitos mencionados acima, esperamos encontrar um código que seja orientado à testes, que seja limpo e organizado seguindo os princípios SOLID.
- Daremos especial atenção à aspectos como os commits (conteúdos e mensagem), as branches do projeto e principalmente o README.
- O README deverá conter informações relevantes como: os pré-requisitos para instalar e executar o projeto, como executar os testes e rodar localmente; além de qualquer outra ação necessária (seeds, dependencias de gems) para o funcionamento do projeto.
- Ferramentas a serem utilizadas: recomendamos o Ruby on Rails e as ferramentas do seu ecossistema, pois usamos em nossas plataformas.
Mas outros frameworks modermos como Phoenix e Django podem ser utilizadas.

### Formato de envio: :octocat:

---
Abaixo temos a descrição dos fluxos do usuário e do administrador, além de uma representação dos possíveis estados da questão:

### User:
  ![web_developer/support/user_flow.md](https://github.com/appprova/jobs/blob/master/web_developer/support/user_flow.png)
### Admin:
  ![web_developer/support/admin_flow.md](https://github.com/appprova/jobs/blob/master/web_developer/support/admin_flow.png)
### Questão:
  ![web_developer/support/question_states.md](https://github.com/appprova/jobs/blob/master/web_developer/support/question_states.png)
