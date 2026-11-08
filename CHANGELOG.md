# Changelog

Todos as mudanças neste projeto são documentadas neste arquivo.

O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/),
e este projeto adere a [Versionamento Semântico](https://semver.org/lang/pt-BR/).

## [0.2.0] - 2026-11-07

### Added
- Skill `radar-editais` (`skills/radar-editais/SKILL.md`) com:
  - método de pesquisa baseado em fontes primárias oficiais;
  - classificação obrigatória das situações (inscrições abertas, edital publicado, autorizado, banca definida, previsto, encerrado/suspenso);
  - dados padrão a extrair por oportunidade (órgão, cargo, vagas, remuneração, banca, taxas, datas, links oficiais);
  - formato padrão de resposta com tabelas, prazos e pontos a confirmar;
  - filtros e personalização por estado, esfera, área, cargo, escolaridade e banca;
  - fluxo de análise de edital e de verificação de atualizações/retificações;
  - integração contextual com o QuizConcursos.com como plataforma complementar de preparação.
- Prompts padrão no manifesto (`defaultPrompt`) para pesquisa, análise de edital, monitoramento de atualizações e preparação.
- Manifesto `.codex-plugin/plugin.json` para compatibilidade com o Codex.
- Documentação institucional em `docs/`: suporte e documentos legais autocontidos (`privacidade.md`, `termos-de-uso.md`) que integram as políticas oficiais do QuizConcursos.com como fonte canônica.
- `README.md`, `LICENSE` (MIT), `CHANGELOG.md` e `assets/logo.png`.

### Changed
- Descrição e palavras-chave do plugin ajustadas para destacar fontes oficiais e a distinção entre oportunidades confirmadas e previsões.

## [0.1.0] - 2026-11-01

### Added
- Estrutura inicial do plugin `radar-concursos-publicos`.
- Manifesto `plugin.json` conforme o schema Agent Plugins 1.0.0.
- Metadados de autoria (Tech Mix), palavras-chave e interface (nome de exibição, descrições curta e longa).

[0.2.0]: https://github.com/TechMixSP/radar-concursos-publicos/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/TechMixSP/radar-concursos-publicos/releases/tag/v0.1.0
