Descrição do Projeto
---------------------
Este projeto é uma aplicação web que permite ao utilizador carregar ficheiros PDF contendo relatórios médicos e obter como resultado uma versão do documento com dados pessoais censurados (ex: nomes, moradas, documentos, salários, etc.).

A censura é realizada por um modelo de inteligência artificial (Gemini 2.0 da Google), que recebe o conteúdo extraído do PDF e retorna o texto com as informações sensíveis substituídas por asteriscos (*). O texto censurado é então exibido na interface da aplicação.

Tecnologias utilizadas
-----------------------
- Frontend:
  - HTML5
  - CSS3
  - JavaScript (Vanilla)

- Backend:
  - Node.js (Express)
  - Python (PyPDF2 para leitura de PDFs)
  - API Gemini da Google (para censura do conteúdo)

Pré-requisitos
---------------
Antes de executar este projeto, é necessário ter instalado no seu sistema:

- Node.js e npm (https://nodejs.org/)
- Python 3.10+ (https://www.python.org/downloads/)
- Uma chave de API válida para acesso à Gemini API

Instalação e Execução
----------------------

1. Clone este repositório:
   git clone https://github.com/seu-usuario/nome-do-repo.git
   cd nome-do-repo

2. Instale as dependências do Node.js:
   npm install

3. Instale a biblioteca PyPDF2 para Python:
   pip install PyPDF2

4. Substitua a sua chave da API Gemini no ficheiro script.py:
   API_KEY = "SUA_CHAVE_API_AQUI"

5. Inicie o servidor Node.js:
   node index.js

6. Abra o ficheiro index.html no seu navegador ou utilize uma extensão como "Live Server" no VS Code.

7. Carregue um ficheiro PDF e clique em “Submeter” para ver o texto censurado.

Estrutura do Projeto
---------------------
- index.html          → Interface da aplicação
- style.css           → Estilos da interface
- script.js           → Lógica do frontend
- index.js            → Backend Node.js (Express)
- script.py           → Script Python para censura de texto
- uploads/            → Pasta onde os PDFs carregados são temporariamente guardados

Notas Finais
------------
- Certifique-se que o PDF contém texto legível (não funciona com PDFs apenas com imagens digitalizadas).
- A API Gemini pode estar sujeita a limites de uso e custo – consulte a documentação oficial: https://ai.google.dev
- O projeto é apenas para fins educacionais e demonstração de integração entre tecnologias.

Autor: Nsimba Tamaku
Ano: 2025
