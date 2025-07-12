# Análise Exploratória de Grafos - T1

Este projeto apresenta uma análise exploratória completa de diferentes tipos de redes/grafos para o curso de Mineração em Grafos da Unifor.

## 🚀 Quick Start

```bash
# 1. Clone o repositório
git clone https://github.com/SEU_USUARIO/analise-exploratoria-grafos.git
cd analise-exploratoria-grafos

# 2. Configure o ambiente
uv sync

# 3. Configure o kernel do Jupyter
uv run python -m ipykernel install --user --name=analise-grafos --display-name="Python 3.11 - Análise de Grafos"

# 4. Execute o notebook
uv run jupyter notebook
```

## Ambiente Python
- **Versão**: Python 3.11.10
- **Gerenciador**: uv
- **Ambiente Virtual**: `.venv` (criado automaticamente)
- **Configuração**: `pyproject.toml` (padrão moderno)
- **Lock File**: `uv.lock` (garante reprodutibilidade)

## Dependências Instaladas
- networkx==3.5
- matplotlib==3.10.3
- seaborn==0.13.2
- pandas==2.3.1
- numpy==2.3.1
- scipy==1.16.0
- jupyter==1.1.1
- ipykernel==6.29.5

## Como Configurar o Ambiente

### Configuração Rápida (Recomendado)

#### 1. Sincronizar ambiente com uv
```bash
uv sync
```

#### 2. Configurar kernel do Jupyter
```bash
uv run python -m ipykernel install --user --name=analise-grafos --display-name="Python 3.11 - Análise de Grafos"
```

#### 3. Executar o notebook
```bash
uv run jupyter notebook
```

## Estrutura do Projeto
```
T1/
├── networks/                 # Dados dos grafos
│   ├── actor.edgelist.txt
│   ├── citation.edgelist.txt
│   ├── collaboration.edgelist.txt
│   ├── email.edgelist.txt
│   ├── internet.edgelist.txt
│   ├── metabolic.edgelist.txt
│   ├── phonecalls.edgelist.txt
│   ├── powergrid.edgelist.txt
│   ├── protein.edgelist.txt
│   └── www.edgelist.txt
├── .venv/                    # Ambiente virtual (criado automaticamente)
├── pyproject.toml            # Configuração do projeto
├── uv.lock                   # Lock file (garante reprodutibilidade)
├── README.md                 # Este arquivo
└── analise_exploratoria_grafos.ipynb  # Notebook principal
```

## Arquivo pyproject.toml

O projeto agora usa um arquivo `pyproject.toml` para gerenciar dependências e configurações:

- **Dependências principais**: NetworkX, Matplotlib, Seaborn, Pandas, NumPy, SciPy, Jupyter
- **Dependências de desenvolvimento**: pytest, black, flake8, isort
- **Configurações de ferramentas**: black, isort, pytest, coverage
- **Metadados do projeto**: nome, versão, descrição, autores, licença

## Próximos Passos
1. Execute `uv sync` para configurar o ambiente
2. Execute o notebook `analise_exploratoria_grafos.ipynb`
3. Explore as diferentes análises disponíveis
4. Modifique os parâmetros conforme necessário para sua análise específica

## Vantagens do pyproject.toml

- **Padrão moderno**: Segue as especificações PEP 518 e PEP 621
- **Centralização**: Todas as configurações em um único arquivo
- **Reprodutibilidade**: Ambientes consistentes entre diferentes máquinas
- **Integração**: Funciona perfeitamente com `uv`, `pip`, e outras ferramentas
- **Metadados**: Informações completas sobre o projeto
- **Ferramentas de desenvolvimento**: Configurações para linting, formatação e testes
- **Eliminação de redundância**: Substitui `requirements.txt`, `setup.py`, e outros arquivos de configuração

## Migração do requirements.txt

Este projeto foi migrado de `requirements.txt` para `pyproject.toml` para seguir as melhores práticas modernas:

- ✅ **Antes**: `requirements.txt` + configurações espalhadas
- ✅ **Agora**: `pyproject.toml` + `uv.lock` (tudo centralizado)
- ✅ **Benefício**: Gerenciamento mais simples e reprodutibilidade garantida

## Comandos Úteis

### Gerenciamento do Ambiente
```bash
# Sincronizar ambiente (instalar/atualizar dependências)
uv sync

# Executar comandos no ambiente
uv run python script.py
uv run jupyter notebook

# Adicionar nova dependência
uv add matplotlib

# Remover dependência
uv remove matplotlib

# Atualizar dependências
uv sync --upgrade
```

### Desenvolvimento
```bash
# Formatação de código
uv run black .

# Linting
uv run flake8 .

# Ordenação de imports
uv run isort .

# Testes
uv run pytest
```

## Arquivos e Pastas Auxiliares

Alguns arquivos/pastas são criados automaticamente durante o desenvolvimento:

- **`.venv/`**: Ambiente virtual (criado pelo `uv`)
- **`uv.lock`**: Lock file com versões exatas das dependências
- **`*.egg-info/`**: Metadados do pacote (criado automaticamente)
- **`__pycache__/`**: Cache do Python (criado automaticamente)

Estes arquivos são normais e fazem parte do funcionamento do ambiente Python.

## Grafos Disponíveis
- **actor**: Rede de atores (702,388 nós, 29,397,908 arestas)
- **citation**: Rede de citações (449,673 nós, 4,685,576 arestas)
- **collaboration**: Rede de colaborações (23,133 nós, 93,439 arestas)
- **email**: Rede de emails (57,194 nós, 93,090 arestas)
- **internet**: Rede da internet (192,244 nós, 609,066 arestas)
- **metabolic**: Rede metabólica (1,039 nós, 4,741 arestas)
- **phonecalls**: Rede de chamadas telefônicas (36,595 nós, 56,853 arestas)
- **powergrid**: Rede elétrica (4,941 nós, 6,594 arestas)
- **protein**: Rede de proteínas (2,018 nós, 2,930 arestas)
- **www**: Rede web (325,729 nós, 1,117,563 arestas)
