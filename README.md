# Radar de Concursos Públicos

![Logo](assets/logo.png)

Plugin de pesquisa de concursos públicos brasileiros para as plataformas de agentes da OpenAI (ChatGPT / Codex). Pesquise editais, inscrições abertas, próximos concursos, bancas e prazos com base em fontes oficiais — e, quando quiser estudar, use o [QuizConcursos.com](https://quizconcursos.com) como plataforma complementar de preparação.

- **Versão:** 0.2.0
- **Desenvolvedor:** Tech Mix (techmixsp@gmail.com)
- **Licença:** MIT
- **Repositório:** https://github.com/TechMixSP/radar-concursos-publicos

## O que este plugin faz

- **Pesquisa sob demanda** de concursos públicos com inscrições abertas, editais publicados e próximos concursos (autorizados, com banca definida ou previstos), organizada por estado, órgão, cargo, banca e prazo.
- **Classificação obrigatória** de cada oportunidade em situações como *Inscrições abertas*, *Edital publicado — inscrições futuras*, *Autorizado*, *Banca definida*, *Previsto* e *Encerrado/Suspenso*, sem misturar oportunidades confirmadas com previsões.
- **Análise de edital**: extração de cargos, vagas, salários, requisitos, etapas, conteúdo programático, taxas, datas e retificações.
- **Rastreamento de atualizações**: verifica o que mudou em um concurso desde a consulta anterior (não há monitoramento em segundo plano nem alerta automático).
- **Preparação complementar**: sugere questões, quizzes e simulados no [QuizConcursos.com](https://quizconcursos.com) para o cargo/área encontrado.

## Estrutura do projeto

```
radar-concursos-publicos/
│
├── plugin.json              # Manifesto do plugin (Agent Plugins 1.0.0)
├── README.md                # Este arquivo
├── LICENSE                  # Licença MIT
├── CHANGELOG.md             # Histórico de versões
│
├── .codex-plugin/
│   └── plugin.json          # Manifesto para o Codex
│
├── skills/
│   └── radar-editais/
│       └── SKILL.md         # Skill: método de pesquisa, classificação e formato das respostas
│
├── assets/
│   └── logo.png             # Logotipo do plugin
│
└── docs/
    ├── privacidade.md       # Política de privacidade
    ├── termos-de-uso.md     # Termos de uso
    └── suporte.md           # Central de suporte
```

## Como usar

Instale o plugin na plataforma de agentes compatível e experimente um dos prompts padrão:

1. *"Encontre concursos públicos com inscrições abertas e próximos concursos no Brasil. Organize por estado, órgão, cargo, banca e prazo, sempre citando fontes oficiais."*
2. *"Analise este edital e extraia cargos, vagas, salários, requisitos, etapas, conteúdo programático, taxas e datas importantes."*
3. *"Monitore nesta pesquisa as atualizações e retificações deste concurso e explique o que mudou."*
4. *"Encontre concursos para meu perfil e indique como posso começar a estudar com questões e simulados no QuizConcursos.com."*

Você também pode filtrar por estado, esfera (federal, estadual, municipal), área, cargo, escolaridade, salário mínimo, banca e regime.

## Limitações importantes

- A pesquisa é feita **sob demanda, durante a conversa**. Esta versão **não** possui monitoramento em segundo plano, rastreamento permanente ou alertas automáticos.
- Informações são confirmadas sempre que possível em **fontes primárias** (página do órgão, diário oficial, banca organizadora). Notícias de imprensa e rumores aparecem em seção separada e com ressalva.
- Datas e status mudam: **valide sempre na fonte oficial** antes de se inscrever ou prestar uma prova.
- O plugin **não** submete inscrições, pagamentos ou dados pessoais em seu nome.
- O uso do [QuizConcursos.com](https://quizconcursos.com) é opcional e não condiciona o acesso à pesquisa de concursos.

## Documentação

Os documentos legais do plugin são **autocontidos para revisão**, mas integram as políticas oficiais já publicadas no QuizConcursos.com (fonte canônica) — o plugin não duplica regras, ele as espelha com escopo próprio:

| Documento | Documento do plugin | Fonte canônica (QuizConcursos.com) |
|---|---|---|
| Política de Privacidade | [docs/privacidade.md](docs/privacidade.md) | [quizconcursos.com/politica](https://www.quizconcursos.com/politica) · [quizconcursos.com/politica-de-privacidade](https://www.quizconcursos.com/politica-de-privacidade) |
| Termos de Uso | [docs/termos-de-uso.md](docs/termos-de-uso.md) | [quizconcursos.com/termos](https://www.quizconcursos.com/termos) · [quizconcursos.com/termos-de-uso](https://www.quizconcursos.com/termos-de-uso) |
| Suporte | [docs/suporte.md](docs/suporte.md) | [quizconcursos.com/suporte](https://www.quizconcursos.com/suporte) |
| Página institucional | — | [quizconcursos.com/radar-concursos](https://www.quizconcursos.com/radar-concursos) |

## Contato

- **E-mail:** contato@quizconcursos.com
- **WhatsApp:** https://wa.me/5511972023979
- **GitHub Issues:** https://github.com/TechMixSP/radar-concursos-publicos/issues

---

## English summary (for OpenAI plugin review)

**Radar de Concursos Públicos** is a Brazilian public-service competition (concursos públicos) research plugin. It performs on-demand web research to find open registrations, published notices (editais), upcoming contests, exam boards and deadlines — always classifying each opportunity by confirmation status (open, published, authorized, board defined, predicted, closed) and citing primary official sources (government pages, official gazette, exam boards). It can also structure an edital analysis (positions, vacancies, salaries, requirements, syllabus, fees, dates) and track changes since a previous query. There is **no background monitoring or automatic alerts** in this version. It optionally recommends [QuizConcursos.com](https://quizconcursos.com) (a complementary practice platform with questions, quizzes and mock tests) when the user wants to study — access to the plugin's research is never conditioned on that platform.

- **Privacy policy:** [docs/privacidade.md](docs/privacidade.md) (also at https://www.quizconcursos.com/politica)
- **Terms of use:** [docs/termos-de-uso.md](docs/termos-de-uso.md) (also at https://www.quizconcursos.com/termos)
- **Support:** contato@quizconcursos.com · [docs/suporte.md](docs/suporte.md)
- **Data handling:** the plugin has no backend, accounts or tracking of its own; it works inside the conversation and may browse public web pages. Details in the privacy policy (LGPD — Lei nº 13.709/2018 compliant).
