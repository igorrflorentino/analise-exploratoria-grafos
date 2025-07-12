# Ambiente Python - Mineração em Grafos T1

## Configuração do Ambiente

Este projeto utiliza o **uv** para gerenciamento de dependências e ambientes virtuais.

### Ambiente Virtual
- **Nome**: `.mineração-grafos-T1` (oculto)
- **Localização**: `./.mineração-grafos-T1/`
- **Python**: 3.11.10

### Como ativar o ambiente

```bash
# Navegar para o diretório do projeto
cd /Users/igorflorentino/Coding/my_repos/Unifor/MineraçãoEmGrafos/T1

# Ativar o ambiente virtual
source .mineração-grafos-T1/bin/activate
```

### Dependências Principais

- **NetworkX** 3.5 - Para análise de grafos
- **Matplotlib** 3.10.3 - Para visualização
- **Seaborn** 0.13.2 - Para visualização estatística
- **Pandas** 2.3.1 - Para manipulação de dados
- **NumPy** 2.3.1 - Para computação numérica
- **SciPy** 1.16.0 - Para computação científica
- **Jupyter** 1.1.1 - Para notebooks interativos
- **IPykernel** 6.29.5 - Para kernels Jupyter

### Dependências de Desenvolvimento

- **Pytest** 8.4.1 - Para testes
- **Black** 25.1.0 - Para formatação de código
- **Flake8** 7.3.0 - Para linting
- **Isort** 6.0.1 - Para organização de imports

### Kernel Jupyter

Um kernel Jupyter foi instalado com o nome:
- **Nome interno**: `mineracao-grafos-T1`
- **Nome de exibição**: "Mineração em Grafos T1"

Para usar o kernel no VS Code ou Jupyter Lab, selecione "Mineração em Grafos T1" na lista de kernels disponíveis.

### Comandos Úteis

```bash
# Verificar pacotes instalados
uv pip list

# Instalar novos pacotes
uv pip install nome-do-pacote

# Instalar dependências do projeto
uv pip install -e .

# Instalar dependências de desenvolvimento
uv pip install -e ".[dev]"

# Executar testes
pytest

# Formatar código
black .

# Verificar estilo do código
flake8 .

# Organizar imports
isort .
```

### Estrutura do Projeto

```
.
├── analise_exploratoria_grafos.ipynb  # Notebook principal
├── networks/                          # Datasets de grafos
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
├── pyproject.toml                     # Configuração do projeto
├── uv.lock                           # Lock file das dependências
├── README.md                         # Documentação do projeto
└── AMBIENTE_SETUP.md                 # Este arquivo
```

### Notas Importantes

1. **Sempre ative o ambiente** antes de trabalhar no projeto
2. **Use o kernel correto** nos notebooks Jupyter
3. **Mantenha as dependências atualizadas** conforme necessário
4. **Execute os testes** antes de fazer commits importantes

### Resolução de Problemas

Se houver problemas com o ambiente:

1. Desative o ambiente atual: `deactivate`
2. Remova o diretório do ambiente: `rm -rf .mineração-grafos-T1`
3. Recrie o ambiente: `uv venv .mineração-grafos-T1`
4. Reative: `source .mineração-grafos-T1/bin/activate`
5. Reinstale as dependências: `uv pip install -e ".[dev]"`
6. Reinstale o kernel: `python -m ipykernel install --user --name=mineracao-grafos-T1 --display-name="Mineração em Grafos T1"`
