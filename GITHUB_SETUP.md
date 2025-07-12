# 🚀 Enviando para o GitHub

## Passo 1: Criar Repositório no GitHub

1. Acesse: https://github.com/new
2. Nome do repositório: `analise-exploratoria-grafos`
3. Descrição: `Análise exploratória de grafos para o curso de Mineração em Grafos - Unifor`
4. Deixe como **Público** (ou Privado se preferir)
5. **NÃO** marque "Add a README file" (já temos um)
6. **NÃO** marque "Add .gitignore" (já temos um)
7. Clique em "Create repository"

## Passo 2: Conectar Repositório Local ao GitHub

Execute os comandos abaixo (substitua `SEU_USUARIO` pelo seu usuário do GitHub):

```bash
# Adicionar remote origin
git remote add origin https://github.com/SEU_USUARIO/analise-exploratoria-grafos.git

# Enviar código para o GitHub
git push -u origin main
```

## Passo 3: Verificar

Acesse seu repositório no GitHub e verifique se todos os arquivos foram enviados corretamente.

## 📁 Estrutura do Repositório

```
analise-exploratoria-grafos/
├── networks/                 # Datasets dos grafos
├── .gitignore               # Arquivos ignorados pelo Git
├── .python-version          # Versão do Python
├── README.md                # Documentação principal
├── analise_exploratoria_grafos.ipynb  # Notebook de análise
├── pyproject.toml           # Configuração do projeto
├── uv.lock                  # Lock file das dependências
└── GITHUB_SETUP.md          # Este arquivo
```

## 🔧 Comandos Git Úteis

```bash
# Ver status
git status

# Adicionar arquivos modificados
git add .

# Fazer commit
git commit -m "descrição das mudanças"

# Enviar para o GitHub
git push

# Ver histórico
git log --oneline

# Ver remotes
git remote -v
```

## 🌟 Próximos Passos

1. **README.md**: Atualize com sua informação pessoal
2. **Issues**: Crie issues para futuras melhorias
3. **Branches**: Use branches para novas funcionalidades
4. **Releases**: Crie releases para versões estáveis
5. **Documentação**: Adicione mais documentação conforme necessário

## 📊 Sobre o Projeto

Este projeto contém:
- **10 redes diferentes** para análise
- **Análises completas**: propriedades básicas, centralidade, comunidades
- **Visualizações**: diferentes layouts e representações
- **Ambiente moderno**: Python 3.11 + uv + pyproject.toml
- **Reprodutibilidade**: uv.lock garante ambientes idênticos

---

Após enviar para o GitHub, você pode deletar este arquivo:
```bash
rm GITHUB_SETUP.md
git add .
git commit -m "docs: remove setup instructions"
git push
```
