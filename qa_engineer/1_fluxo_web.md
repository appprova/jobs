# Responder e entregar uma ativdade

O objetivo da automação desse fluxo é acessar a plataforma do aluno, preencher o perfil corretamente, responder à todas as questões de uma atividade, e entregá-la.

## Você deve acessar a plataforma através do nosso ambiente de [staging](http://mobile.stg.appprova.com.br/)

Para completar o fluxo, podem ser necessários alguns passos adiconais como:

- Criação de uma conta como aluno;
- Preenchimento do perfil corretamente (estado, cidade escola, turma - e matrícula, se aplicável);
- Aceitar os termos de uso e politica de privacidade da plataforma;

Para cada passo do fluxo, podem existir casos _edge_, como por exemplo:
- Email já em uso;
- Perfil preenchido incorretamente;
- Responder uma pergunta sem marcar alternativa;
- Responder um simulado após o término do tempo disponível
- ...

