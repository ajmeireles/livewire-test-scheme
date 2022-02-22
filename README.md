### Livewire, Teste.

O objetivo deste teste é validar expressamente o seu conhecimento e aptidão necessária.

#### Remuneração

Para que o teste seja remunerado você deve **gravar todo processo de criação do teste sem cortes.**

##### Stack

- Laravel 9
- PHP 8.1
- Livewire
- AlpineJs

##### Requerimentos

- PHP 8.1 – **obrigatório**
- Laravel 8 – **obrigatório**
- Laravel Livewire – **obrigatório**
- AlpineJs – **obrigatório**
- TailwindCss – **obrigatório** 
- Laravel Sail (Docker) – *opcional*
- Laravel Breeze – **obrigatório**
- **Todo código deve ser escrito em inglês e seguindo a PSR12**

##### Telas de Autenticação (Baseado em *Laravel Breeze*)

- Registro, com: nome, e-mail e senha
- Login
- Recuperação de senha **(se via Docker, use MailHog)**

##### Funcionalidades Esperadas:

1. Crie uma tela para acesso via rota “/dashboard” chamada “dashboard”.

2. Esta tela deve ser composta por TailwindCss de forma organizada.

3. A proposta da tela de dashboar deve ser esta: https://i.imgur.com/iNVW0cz.png

4. Nesta tela deve haver um botão, na div centralizada (abaixo de: “You’re logged in”), que ao ser clicado haja uma requisição (via Livewire & HTTP) para uma API geradora de lorem, exemplo: 
https://baconipsum.com/api/?type=meat-and-filler

5. Quando o click ocorrer a requisição deve ser realizada e o resultado do texto (Lorem) deve ser armazenado em uma variável do Livewire para ser exibido em baixo do botão: https://i.imgur.com/bYPZ1Wd.png – **CADA CLICK DEVE GERAR UM TEXTO DIFERENTE.**

6. Ao contabilizar 10 clicks consecultivos as requisições devem ser interrompidas gerando um alerta "Sweet Alert" (tipo danger): https://sweetalert.js.org/guides/ ao usuário com alguma frase sugestiva sobre o "limite de clicks".

7. O botão deve ser desabilitado enquanto a requisição estiver em andamento.

8. Enquanto o botão não for clicado, não deve ser exibido nenhum texto.


##### Outros (observações):

1. Crie um teste de unidade para validar basicamente a funcionalidade da aplicação.

2. O teste deve ser conceituado sobre o esquema de testes do Livewire.

3. O teste deve ter validar sucessos e também falhas.

##### Entrega do Teste:

- **Hospede o teste em um repositório do GitHub e envie o link do repositório e também o link da gravação do teste (conforme explicado na sessão “Remuneração”).** Lembre-se que tudo será levado em conta a ser analisado.
