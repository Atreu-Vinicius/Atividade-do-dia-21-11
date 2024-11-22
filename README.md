# Configuracao do Aplicativo React com Reactstrap

## Objetivo

Neste exercicio, o objetivo foi configurar um projeto React para usar o pacote **Reactstrap**, que oferece componentes **Bootstrap** prontos para usar em React. Ao final da atividade, o aluno sera capaz de:

1. Configurar o projeto React para usar o Reactstrap.
2. Utilizar componentes Reactstrap em um aplicativo React.
3. Criar uma barra de navegacao (Navbar) personalizada com Reactstrap.

## Passos Realizados

### 1. Instalacao do Reactstrap e Dependencias

Para configurar o projeto, foram instalados os pacotes necessarios com os seguintes comandos:

```bash
npm install reactstrap react react-dom
npm install --save bootstrap
npm install react-popper @popperjs/core
```

2. Configuracao do Bootstrap
Foi adicionada a importacao do arquivo CSS do Bootstrap no arquivo index.js para aplicar o estilo global:

javascript
Copiar código
import 'bootstrap/dist/css/bootstrap.min.css';
3. Adicao de uma Barra de Navegacao (Navbar)
No arquivo App.js, foi criado um componente de Navbar utilizando o Reactstrap. A barra de navegacao foi personalizada para incluir o nome do aluno.

Codigo no App.js:

javascript
Copiar código
import { Navbar, NavbarBrand } from 'reactstrap';

function App() {
  return (
    <div className="App">
      <Navbar dark color="primary">
        <div className="container">
          <NavbarBrand href="/">Ristorante Con Fusion</NavbarBrand>
          <div>Aluno: Seu Nome Aqui</div>
        </div>
      </Navbar>
    </div>
  );
}

export default App;
Substitua "Seu Nome Aqui" pelo seu nome.

4. Atualizacao do README.md
O arquivo README.md foi atualizado com um resumo dos passos realizados para configurar o Reactstrap no projeto. Alem disso, uma imagem foi capturada para ilustrar a barra de navegacao com o nome do aluno.

Exemplo de entrada no README.md:

markdown
Copiar código
### Imagem da Barra de Navegacao
![Texo alternativo](img_navbar.png)
A imagem da barra de navegacao foi adicionada a documentacao.

5. Commit no Git
Após as alteracoes, o repositório foi atualizado com o commit de configuracao do React:

bash
Copiar código
git add .
git commit -m "Configurando o React"
git push
Conclusao
Neste exercicio, conseguimos configurar o React para usar o Reactstrap, adicionando componentes do Bootstrap ao aplicativo. A barra de navegacao foi criada com o nome do aluno e o repositório foi atualizado corretamente.

Desenvolvido por Seu Nome.

perl
Copiar código

### Como Usar:

1. Substitua "Seu Nome Aqui" pelo seu nome no arquivo `App.js`.
2. Insira a imagem da barra de navegacao no `README.md` no local apropriado, como mostrado no exemplo.
3. Realize os passos no terminal para instalar as dependencias, atualizar o codigo e fazer o commit.

Resumo do código:

1. <Navbar dark color="primary">: Cria uma barra de navegação com o tema escuro (dark) e a cor primária do bootstrap.

2.<div className="container">: Agrupa os elementos da navbar dentro de um container, o que ajuda a manter o conteúdo alinhado e responsivo.

3.<NavbarBrand href="/">Ristorante Con Fusion</NavbarBrand>: Adiciona o nome do site ou marca, "Ristorante Con Fusion", que também serve como um link para a página inicial (/).

4.<div>Aluno: Fulano de Tal</div>: Exibe o nome do aluno ("Fulano de Tal") dentro da barra de navegação. Este texto pode ser substituído pelo nome do aluno real.
