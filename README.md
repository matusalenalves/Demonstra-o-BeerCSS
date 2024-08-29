# Demonstração do BeerCSS para o ERCEMAPI 2024

Este é um projeto de uma página feito nos moldes de um portfólio de desenvolvedor. Seu propósito é demonstrar como construir páginas bonitas, responsivas e interativas com o BeerCSS de maneira ágil. Será apresentado no ERCEMAPI 2024 no dia 12 de setembro durante o minicurso "Design Web Intuitivo: Potencializando Projetos com Material Design e BeerCSS".

Este é o código-fonte do meu portfólio de desenvolvedor, construído com BeerCSS e seguindo as métricas do Material Design. Este projeto é ideal para desenvolvedores que desejam criar um portfólio moderno e responsivo.

## Pré-requisitos

Antes de começar, você precisará ter as seguintes ferramentas instaladas em sua máquina:

- [Visual Studio Code (VS Code)](https://code.visualstudio.com/) - Um editor de código leve, mas poderoso.
- [Git](https://git-scm.com/) - Para clonar o repositório do GitHub.

## Como utilizar este projeto

Siga os passos abaixo para configurar o projeto na sua máquina:

### 1. Clonar o repositório

Abra o terminal e execute o seguinte comando para clonar este repositório:

```bash
git clone https://github.com/matusalenalves/Demo_BeerCSS.git
```

### 2. Navegar até o diretório do projeto

Após clonar o repositório, os arquivos do projeto estarão dentro de uma nova pasta no seu sistema. Para trabalhar com esses arquivos, você precisa "entrar" nessa pasta no terminal. Aqui está um guia passo a passo:

#### 2.1. Identificar o nome do diretório (pasta): 

   Quando você clona um repositório, ele é baixado para uma pasta cujo nome é, por padrão, o mesmo nome do repositório no GitHub. Nesse caso, o nome do depositório no Github é **Demo_BeerCSS**, ou seja, uma nova pasta com o nome **Demo_BeerCSS** será criada na sua máquina.

#### 2.2. Usar o comando 'cd': 

   No terminal, você pode usar o comando cd (que significa "change directory" ou "mudar de diretório") para acessar essa nova pasta. O formato básico do comando é:

   ```bash
   cd nome-da-pasta
   ```

   Neste caso, a pasta se chama **Demo_BeerCSS**, então: 

   ```bash
   cd Demo_BeerCSS
   ```

   Depois de executar esse comando, o terminal estará "dentro" da pasta do projeto, e você poderá executar comandos específicos para esse projeto, como abrir o código no VS Code, instalar dependências, etc.

   **Observação:** Se você clonou o repositório em uma localização diferente da sua pasta de usuário padrão, você precisará especificar o caminho completo para a pasta. Por exemplo:

   ```bash
   cd /caminho/para/sua/pasta/Demo_BeerCSS
   ```

### 3. Abrir o projeto no VS Code

No terminal, dentro do diretório do projeto, execute o seguinte comando:

```bash
code .
```
**Explicação:**
'code': Este comando abre o VS Code a partir do terminal.    
'.': O ponto '.' representa o diretório atual. Assim, este comando abrirá o diretório atual (que deve ser o diretório do seu projeto) diretamente no VS Code.
Se o comando code não funcionar, pode ser que ele não esteja configurado no seu PATH. Você pode configurá-lo facilmente:
1. Abra o VS Code.
2. Pressione **Ctrl + Shift + P** (ou **Cmd + Shift + P** no macOS) para abrir a paleta de comandos.
3. Digite e selecione "Shell Command: Install 'code' command in PATH".    
4. Pressione **Enter** para instalar o comando.

Após executar o comando, o VS Code abrirá com o seu projeto carregado. No painel à esquerda, você verá a estrutura de pastas e arquivos do projeto.

### 4. Instalar dependências

Você pode utilizar o BeerCSS tanto via CDN quanto via NPM, conforme descrito abaixo:

#### 4.1. Uso do BeerCSS via CDN:

   Se você prefere usar o BeerCSS via CDN, pode adicionar o seguinte código no arquivo HTML do seu projeto, geralmente dentro da seção `<head>`:

   **Com HTML:**

   ```html
   <link href="https://cdn.jsdelivr.net/npm/beercss@3.6.13/dist/cdn/beer.min.css" rel="stylesheet" />
   <script type="module" src="https://cdn.jsdelivr.net/npm/beercss@3.6.13/dist/cdn/beer.min.js"></script>
   <script type="module" src="https://cdn.jsdelivr.net/npm/material-dynamic-colors@1.1.2/dist/cdn/material-dynamic-colors.min.js"></script>
   ```

   **Com CSS:**

   ```css
   @import "https://cdn.jsdelivr.net/npm/beercss@3.6.13/dist/cdn/beer.min.css";
   ```

   **Com Javascript:**

   ```javascript
   import "https://cdn.jsdelivr.net/npm/beercss@3.6.13/dist/cdn/beer.min.js";
   import "https://cdn.jsdelivr.net/npm/material-dynamic-colors@1.1.2/dist/cdn/material-dynamic-colors.min.js";
   ```

#### 4.2. Instalação via NPM:

   Se você preferir gerenciar as dependências do projeto via NPM, execute os seguintes comandos para instalar o BeerCSS e o Material Dynamic Colors:

   ```bash
   npm i beercss
   npm i material-dynamic-colors
   ```

   **Importando no JavaScript:**

   Após a instalação via NPM, você pode importar o BeerCSS e o Material Dynamic Colors no seu arquivo JavaScript da seguinte maneira:

   ```bash
   // Importando como window.beercss e window.materialDynamicColors
   import "beercss";
   import "material-dynamic-colors";
   ```
   Isso permitirá que você utilize o BeerCSS e o Material Dynamic Colors diretamente no seu projeto com suporte completo ao JavaScript ES Modules.