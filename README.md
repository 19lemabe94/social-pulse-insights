# SocialPulse-Insights

### Transformando Dados de Redes Sociais em Insights Acionáveis

O **SocialPulse-Insights** é uma ferramenta desenvolvida em Python para extrair, processar e analisar dados de redes sociais. O objetivo do projeto é ajudar empresas a entender a percepção de suas marcas e produtos, identificando tendências, monitorando a reputação e extraindo insights valiosos a partir do "pulso" da internet.

---

### 🌟 Funcionalidades Principais

- **Coleta de Dados:** Utiliza APIs oficiais para extrair posts e comentários de plataformas como Twitter (X), Reddit e YouTube.
- **Processamento e Limpeza de Texto:** Remove caracteres especiais, URLs, menções e hashtags para preparar o texto para análise.
- **Análise de Sentimento:** Classifica as menções como **Positivas**, **Negativas** ou **Neutras**, fornecendo uma visão geral sobre o sentimento do público.
- **Extração de Insights:** Identifica as hashtags mais populares, as palavras-chave mais mencionadas e o volume de posts ao longo do tempo.
- **Visualização de Dados:** Transforma os resultados da análise em visuais fáceis de entender, como nuvens de palavras e gráficos.

---

### 💻 Tecnologias Utilizadas

- **Linguagem:** Python 3
- **Bibliotecas Principais:**
  - `tweepy`: Para interagir com a API do Twitter (X).
  - `pandas`: Para manipulação e análise dos dados em formato de tabela.
  - `textblob`: Para análise de sentimento (com suporte a português).
  - `matplotlib` / `seaborn`: Para a criação de gráficos.
  - `wordcloud`: Para gerar nuvens de palavras.

---

### 🚀 Como Usar o Projeto

#### Pré-requisitos
- Python 3.x instalado
- Git instalado
- Uma conta de desenvolvedor no Twitter (X) com as chaves de API.

#### 1. Clonar o Repositório

```bash
git clone https://github.com/19lemabe94/social-pulse-insights.git
cd social-pulse-insights
```

#### 2. Criar e Ativar o Ambiente Virtual

```bash
python -m venv venv
# Ativar no Linux/Mac
source venv/bin/activate
# Ativar no Windows (Prompt de Comando)
venv\Scripts\activate
# Ativar no Windows (PowerShell, se necessário, permita scripts com: Set-ExecutionPolicy -Scope CurrentUser RemoteSigned)
```

#### 3. Instalar Dependências

```bash
pip install -r requirements.txt
```

#### 4. Configurar Credenciais da API
Crie um arquivo `.env` na raiz do projeto com as chaves de acesso da API do Twitter (X) (e outras plataformas que desejar integrar):

```env
TWITTER_API_KEY=xxxxxxxx
TWITTER_API_SECRET=xxxxxxxx
TWITTER_ACCESS_TOKEN=xxxxxxxx
TWITTER_ACCESS_SECRET=xxxxxxxx
```

#### 5. Executar a Ferramenta

```bash
python main.py
```

---

### 📊 Exemplos de Saída

- **Análise de Sentimento:** Gráfico de barras mostrando o percentual de menções positivas, negativas e neutras.
- **Nuvem de Palavras:** Visualização das palavras mais mencionadas nos posts.
- **Timeline de Menções:** Evolução do volume de posts sobre o tema analisado ao longo do tempo.

---

### 📂 Estrutura do Projeto

```
social-pulse-insights/
├─ data/                # Armazena dados brutos e processados
├─ notebooks/           # Jupyter notebooks para testes e análises
├─ src/                 # Código-fonte principal do projeto
│  ├─ collector/        # Scripts de coleta de dados (APIs)
│  ├─ preprocessing/    # Limpeza e tratamento dos textos
│  ├─ analysis/         # Módulos de análise de sentimento e insights
│  ├─ visualization/    # Geração de gráficos e nuvens de palavras
│  └─ utils/            # Funções auxiliares
├─ requirements.txt     # Lista de dependências
├─ main.py              # Script principal para rodar o projeto
├─ .env.example         # Exemplo de configuração de credenciais
└─ README.md            # Documentação do projeto
```

---

### 🤝 Como Contribuir

1. Faça um **fork** do repositório.
2. Crie uma **branch** para sua feature ou correção:
   ```bash
   git checkout -b minha-feature
   ```
3. Faça o **commit** das suas alterações:
   ```bash
   git commit -m "Adiciona nova funcionalidade"
   ```
4. Envie sua branch para o repositório remoto:
   ```bash
   git push origin minha-feature
   ```
5. Abra um **Pull Request**.

---

### 🧩 Dicas & Solução de Problemas (Opcional)

- **PowerShell bloqueando `activate`:**
  ```powershell
  Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
  ```
- **`textblob` sem corpora:** (se precisar)
  ```bash
  python -m textblob.download_corpora
  ```

---

### 📜 Licença

Este projeto é distribuído sob a licença MIT. Consulte o arquivo `LICENSE` para mais informações.

---

### ✨ Autor

Desenvolvido por **[19lemabe94](https://github.com/19lemabe94)** 🚀
