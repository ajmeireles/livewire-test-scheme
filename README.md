### Livewire, Teste.

O objetivo deste teste é validar expressamente o seu conhecimento e aptidão necessária.

**Prazo Objetivo: 2h00**

---

#### Remuneração

Para que o teste seja remunerado você deve **gravar todo processo de criação do teste sem cortes.** - conforme explicação dada via e-mail.

---

##### Stack

- Laravel 9
- PHP 8.1
- Livewire
- AlpineJs

---

##### Requerimentos

- PHP 8.1 – **obrigatório**
- Laravel 8 – **obrigatório**
- Laravel Livewire – **obrigatório**
- TailwindCss – **obrigatório** 
- AlpineJs - **obrigatório** 
- Laravel Sail **(Docker)** – **obrigatório**
- Laravel Breeze – **obrigatório**
- **Todo código deve ser escrito em inglês e seguindo a PSR12**

---

##### Telas de Autenticação (Baseado em *Laravel Breeze*)

- Registro, com: nome, e-mail e senha
- Login
- Recuperação de senha **(use o serviço do MailHog, oferecido pelo Laravel Sail, docker)**

---

##### Preparação

1. Crie uma migração que implemente (crie) uma tabela `limits`

2. Esta tabela deve ser composta por: `id`, `user_id`, `created_at` e `updated_at`

3. Crie um modelador para esta tabela

4. Crie um relacionamento entre a tabela `limits` e a tabela `user` - usando a coluna `user_id`

5. Crie seeders e factories para a tabela `limits` afim de gerar (salvar) dados falsos quando preciso.

---

##### Funcionalidades Esperadas:

1. Crie uma tela para **acesso via rota “/dashboard” chamada “dashboard”.**

2. Esta tela **deve ser composta por TailwindCss** de forma organizada.

3. **A proposta** da tela de dashboar deve ser esta: https://i.imgur.com/iNVW0cz.png

4. Nesta tela deve haver um botão **(estilizado de qualquer forma, mas usando TailWindCss)**, na div centralizada (abaixo de: “You’re logged in”), que ao ser clicado haja uma requisição (via Livewire & HTTP) para uma API geradora de lorem, exemplo: 
https://baconipsum.com/api/?type=meat-and-filler

5. **Quando o click ocorrer** a requisição deve ser realizada e **o resultado do texto (Lorem) deve ser armazenado em uma variável do Livewire para ser exibido em baixo do botão**: https://i.imgur.com/bYPZ1Wd.png – **CADA CLICK DEVE GERAR UM TEXTO DIFERENTE e o primeiro texto deve ser introduzido com uma transição do AlpineJs para gerar um efeito fade-in e fade-out.**

6. **Ao contabilizar 10 clicks consecultivos** as requisições devem ser interrompidas gerando um alerta "Sweet Alert" **(tipo danger)**: https://sweetalert.js.org/guides/ **(instale o pacote e gere alertas via eventos do Livewire)** ao usuário com alguma frase sugestiva sobre o "limite de clicks", **juntamente com o armazenamento de um novo registro no banco de dados (tabela `limits`) sobre quando ocorreu o limite.**

7. O botão deve ser desabilitado **enquanto** a requisição estiver em andamento.

8. **Enquanto o botão não for clicado** não deve ser exibido nenhum texto.

---

##### Outros (observações):

1. Crie um teste de unidade para validar basicamente a funcionalidade da aplicação.

2. Crie um teste de unidade para validar o relacionamento entre `user` e `limits`

3. Os testes **devem validar casos de sucessos e também de falhas/erros.**

---

##### Entrega do Teste:

- **Hospede o teste em um repositório do GitHub (público) e envie o link do repositório e também o link da gravação do teste (conforme explicado na sessão “Remuneração”).**
