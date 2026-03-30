# Changelog

Todas as mudanças notáveis deste projeto serão documentadas neste arquivo.

Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.0.0/).

## [v0.1.1] — 2026-03-30

### Added
- Menu de contexto do Windows (clique-direito em pastas)
- Opções "Converter DNG → JPG" e "Converter DNG → PNG" no Explorer
- Modo CLI com subcomandos: `convert`, `install`, `uninstall`
- Busca recursiva em subpastas (automática no CLI, checkbox na GUI)
- Comando `install` / `uninstall` para gerenciar menu de contexto

### Changed
- Lógica de conversão extraída para funções standalone reutilizáveis
- GUI refatorada para usar funções compartilhadas com CLI

## [v0.1.0] — 2026-03-30

### Added
- Interface gráfica com tkinter para conversão de DNG
- Seleção de pasta inteira ou arquivos individuais
- Opção de formato de saída: JPG ou PNG
- Controle de qualidade JPG (1–100, padrão 95)
- Conversão em cascata: rawpy → Pillow (TIFF) → ImageMagick
- Barra de progresso com log detalhado
- Thread separada para conversão (GUI responsiva)
- README.md com documentação completa
- CLAUDE.md com instruções de desenvolvimento
