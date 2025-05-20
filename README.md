# Desafio dos 7 Erros - Docker, Node.js e MongoDB

Este é um desafio para testar seus conhecimentos em Docker, Node.js e MongoDB. A aplicação contém 7 erros que impedem seu funcionamento correto.

## Descrição do Desafio

Você recebeu uma aplicação Node.js que deve se conectar a um banco de dados MongoDB. Ambos devem ser executados em containers Docker usando o Docker Compose.

No entanto, existem 7 erros nos arquivos de configuração que impedem a aplicação de funcionar corretamente. Seu trabalho é:

1. Identificar os 7 erros
2. Corrigir cada um deles
3. Garantir que a aplicação funcione corretamente

## Estrutura do Projeto

```
./
├── app/
│   ├── index.js         # Código da aplicação Node.js
│   ├── package.json     # Dependências da aplicação
│   └── Dockerfile       # Dockerfile para construir a imagem da aplicação
└── docker-compose.yml   # Arquivo de configuração do Docker Compose
```

## Instruções

1. Faça um fork deste repositório para sua conta GitHub
2. Clone o repositório para sua máquina local
3. Analise os arquivos do projeto e identifique os 7 erros
4. Corrija cada erro encontrado
5. Execute a aplicação com `docker-compose up`
6. Verifique se a aplicação está funcionando acessando:
   - http://localhost:3000 (página principal)
   - http://localhost:3000/itens (API para listar itens)
7. Teste a criação de um item com:
   ```
   curl -X POST http://localhost:3000/itens \
     -H "Content-Type: application/json" \
     -d '{"nome": "Item de teste", "descricao": "Descrição do item de teste"}'
   ```
8. Após corrigir todos os erros, faça um pull request para o repositório original

## Como fazer um Fork e Pull Request

### Fork do Repositório

1. Acesse o repositório original no GitHub
2. No canto superior direito da página, clique no botão "Fork"
3. Selecione sua conta para criar o fork
4. Aguarde o processo de fork ser concluído

### Clone do Repositório

1. No seu fork, clique no botão verde "Code"
2. Copie a URL do repositório
3. Abra o terminal e execute:
   ```
   git clone [URL_DO_SEU_FORK]
   cd [NOME_DO_REPOSITORIO]
   ```

### Fazendo as Alterações

1. Crie uma nova branch para suas alterações:
   ```
   git checkout -b correcao-desafio
   ```
2. Faça as correções necessárias nos arquivos
3. Adicione as alterações:
   ```
   git add .
   ```
4. Faça o commit das alterações:
   ```
   git commit -m "Correção dos 7 erros do desafio"
   ```
5. Envie as alterações para o seu fork:
   ```
   git push origin correcao-desafio
   ```

### Criando o Pull Request

1. Acesse seu fork no GitHub
2. Clique no botão "Compare & pull request" que aparecerá no topo
3. Verifique se a base repository é o repositório original e o head repository é o seu fork
4. Adicione um título descritivo como "Correção dos 7 erros do desafio"
5. No corpo do PR, liste os erros encontrados e como você os corrigiu
6. Clique em "Create pull request"

## Solução

- Após completar o desafio, inclua no pull request um arquivo `solucao.md` listando cada erro encontrado, como você o corrigiu e seu nome e RA. 
- Na descrição do pull request coloque seu Nome e RA

Bom Desafio a Todos!