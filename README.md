# Website Institucional Sustentável — Enactus UFRA 🚀

> **Status do Projeto:** Em Desenvolvimento 🛠️

Este repositório contém a camada de desenvolvimento do novo website institucional da **Enactus UFRA** (Universidade Federal Rural da Amazônia). O projeto foi idealizado e construído com foco em centralizar os projetos de impacto socioambiental, notícias, editais e a história do time, servindo como um portal oficial para a comunidade acadêmica e parceiros externos.

---

## 🎯 O Desafio do Legado e Engenharia de Soluções

O maior desafio técnico deste projeto não foi apenas a codificação do layout, mas sim a **sustentabilidade a longo prazo**. 

Em ambientes universitários de impacto social, a rotatividade de membros é naturalmente alta. Optar por frameworks complexos (como React ou Next.js) criaria um gargalo tecnológico, fazendo com que o site "morresse" assim que os desenvolvedores atuais saíssem do projeto, devido à falta de mão de obra técnica especializada para manutenção.

### A Solução Híbrida (Low-Code / No-Code Profissional)
Para mitigar esse risco e entregar um **legado real e autônomo**, a stack foi arquitetada utilizando o **WordPress** integrado ao construtor visual **Elementor** sobre o ecossistema leve do tema **Hello Elementor**. 
* **Para quem fica (O Time):** A atualização de posts, novos projetos e gerenciamento de membros é feita de forma visual e intuitiva (interface amigável em nível de editor de texto).
* **Para quem desenvolve (Nossa Equipe):** O Git rastreia toda a estrutura de customização, arquivos de estilos personalizados (CSS), templates de páginas exportados e controle de versionamento dos arquivos do ecossistema do site.

---

## 🛠️ Stack Tecnológica e Ferramentas

- **Core do Sistema:** WordPress (Ambiente CMS)
- **Design & Layout:** Elementor (Componentização visual e responsividade)
- **Tema Base:** Hello Elementor (Tema minimalista e otimizado para performance)
- **Banco de Dados:** MySQL
- **Ambiente Local:** LocalWP / Docker
- **Versionamento:** Git & GitHub

---

## 📁 Estrutura do Repositório

Para manter o repositório limpo e evitar versionar o "core" nativo do WordPress (que recebe atualizações constantes de terceiros), este repositório rastreia essencialmente a pasta de customização do projeto (`/wp-content/`):

```text
├── wp-content/
│   ├── themes/
│   │   └── hello-elementor/      # Tema base do projeto
│   ├── templates/                # Arquivos .json das páginas exportadas (para sincronização)
│   ├── plugins/                  # Plugins estritamente necessários para o funcionamento
│   └── .gitignore                # Regras de exclusão (ignora pastas de uploads locais)
└── README.md                     # Documentação do projeto
