# Commits

### TIPOS

```feat``` - Commits do tipo feat indicam que seu trecho de código está incluindo um novo
recurso (se relaciona com o MINOR do versionamento semântico).

```fix``` - Commits do tipo fix indicam que seu trecho de código commitado está solucionando um problema (bug fix),
(se relaciona com o PATCH do versionamento semântico).

```test``` - Commits do tipo test são utilizados quando são realizadas alterações em testes, seja criando, 
alterando ou excluindo testes unitários. (Não inclui alterações em código).

```build``` - Commits do tipo build são utilizados quando são realizados modificações em arquivos de build e
dependências.

```docs``` - Commits do tipo docs indicam que houveram mudanças na documentação, como por exemplo no Readme do seu
repositório. (Não inclui alterações em código).

```perf``` - Commits do tipo perf servem para identificar quaisquer alterações de código que estejam relacionadas
a performance.

```style``` - Commits do tipo style indicam que houveram alterações referentes a formatações de código, semicolons,
trailing, spaces, lint... (Não inclui alterações em código).

```ci``` - Commits do tipo ci indicam mudanças relacionadas a integração contínua (continuous integration).

```chore``` - Commits do tipo chore indicam atualizações de tarefas de build, configurações de administrador,
pacotes... como por exemplo adicionar um pacote no gitignore. (Não inclui alterações em código).

<br/>

### RECOMENDAÇÕES

- Adicione um título consciente com o título  do conteúdo;
- Recomendamos que na primeira linha deve ter no máximo 4 palavras;
- Para descrever com detalhes, usar a descrição do commit;
- Usar um emoji no início da mensagem de commit representando sobre o commit;
- Um link precisa ser adicionado em sua forma mais autêntica, ou seja: sem encurtadores de link e
links afiliados;

<br/>

### EXEMPLOS

```
  git commit -m "type: message..."
  git commit -m "test: add test of creaet product automation"
  git commit -m "fix: remove getPayment() wrong attribute"
```
