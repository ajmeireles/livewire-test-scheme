### Esquema de Testes, TALL Stack.

O objetivo deste teste é validar expressamente o seu conhecimento e aptidão necessária a vaga proposta.

---

### Sobre o Teste

- Prazo de Conclusão: 2h00
- Remuneração:
   - Valor informado por e-mail
   - Para a remuneração ser efetivada todo teste deve ser gravado sem edições ou cortes.
- Entrega do Teste: Crie um repositório público e hospede a aplicação.

---

### Requerimentos

- PHP 8.1 – **obrigatório**
- Laravel 8 (ou 9) – **obrigatório**
- Laravel Livewire – **obrigatório**
- TailwindCss – **obrigatório**
- AlpineJs - **obrigatório**
- Laravel Sail **(Docker)** – **obrigatório**
- Laravel Breeze – **obrigatório (scaffolding Livewire)**

**Se o código for escrito em inglês será um diferencial! :)**

---

### Telas de Autenticação (Baseado em *Laravel Breeze*)

- Registro, com: nome, e-mail e senha
- Login
- Recuperação de Senha

---

### Preparação

1. Crie uma migração que implemente _(crie)_ uma tabela `limits`

2. Esta tabela deve ser composta por: `id`, `user_id`, `created_at` e `updated_at`

3. Crie um modelador para esta tabela (Limits).

4. Crie um relacionamento (1 => N) entre a tabela `limits` e a tabela `user` - usando a coluna `user_id`

---

### Funcionalidades Esperadas (Principal)

1. Crie uma tela para **acesso via rota “/dashboard” chamada “dashboard”.**


3. Esta tela **deve ser composta por TailwindCss** de forma organizada - entregue pelo *Laravel Breeze*


5. **A proposta** da tela de dashboar deve ser esta: https://i.imgur.com/iNVW0cz.png


5. Nesta tela deve haver um botão **(estilizado de qualquer forma, mas usando TailwindCss)**, na div centralizada (abaixo de: “You’re logged in”), que ao ser clicado haja uma requisição (via Livewire & HTTP) para uma API geradora de lorem, exemplo:
   https://baconipsum.com/api/?type=meat-and-filler


6. **Quando o click ocorrer** a requisição deve ser realizada e **o resultado do texto (Lorem) deve ser armazenado em uma variável do Livewire para ser exibido em baixo do botão**: https://i.imgur.com/bYPZ1Wd.png – **CADA CLICK DEVE GERAR UM TEXTO DIFERENTE e o primeiro texto deve ser introduzido com uma transição do AlpineJs para gerar um efeito fade-in e fade-out.**


7. **Ao contabilizar 10 clicks consecultivos** as requisições devem ser interrompidas gerando um alerta ao usuário com alguma frase sugestiva sobre o "limite de clicks", **juntamente com o armazenamento de um novo registro no banco de dados (tabela `limits`) sobre quando ocorreu o limite.** (a cada 10 clicks, um registro na tabela `limits` deve ser contabilizado)


8. O botão deve ser desabilitado **enquanto** a requisição estiver em andamento.


9. **Enquanto o botão não for clicado** não deve ser exibido nenhum texto.

---

### Finalização e Validação

**Obs.: Esta etapa só deve ser realizada caso você possua conhecimento suficiente.**

1. Crie um teste de unidade para validar a funcionalidade da aplicação.

2. Crie um teste de unidade para validar o relacionamento entre `user` e `limits`

3. Os testes **devem validar casos de sucessos e também de falhas/erros.**
