Desafio Técnico
=================

### Descrição:

Escolha uma das aplicações:
  - [Ruby on Rails](https://github.com/gothinkster/rails-realworld-example-app)
  - [CakePHP](https://github.com/gothinkster/cakephp-realworld-example-app)
  - [Elixir + Phoenix](https://github.com/gothinkster/elixir-phoenix-realworld-example-app)

  Para Dockerizar e implementar o deploy para o ambiente de cluster Kubernetes.

---
- Manter a simplicidade no Dockerfile
  - Dockerfile genérico para vários environments **se possível**
  - Tamanho da imagem final reduzido **se possível**

- Para o deploy da aplicação no Kubernetes implemente:
  - Deployment
  - Horizontal Pod Autoscaler
  - Ingress ou Balancer
  - Resource Quotas
  - Secrets

---
**Bonus:**

Usando [BCC Tools](https://github.com/iovisor/bcc), investigue a causa de um programa ficar [Off-CPU](http://www.brendangregg.com/offcpuanalysis.html):

- Compile e execute este pequeno [programa](https://gist.github.com/antoniosb/dd79afc4942996fc0b690a459fbbc453)
```
$ gcc -g -fno-omit-frame-pointer -fno-inline -pthread  blocky.c -o blocky
$ ./blocky
```
*Em algumas distros Linux o -pthread é substituído por -lpthread*

Verifique o mal uso de `CPU` feito pelo programa, ele deveria utilizar todos os cores mas por algum motivo acaba gastando muito tempo em apenas 1 só core.

- Objetivos
  - Realizar o profiling da aplicação para verificar o uso de CPU
  - Identificar o tempo gasto em off-CPU
  - Coletar `stack traces` e gerar um gráfico de análise com [FlameGraph](https://github.com/brendangregg/FlameGraph)
