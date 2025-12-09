# Changelog

## [2.1.0] - 2024-12-08

### Fixed
- **Corrigido erro `searchInput.clear is not a function`**: Substituído por `searchInput.fill('')` que é o método correto do Playwright
- **Timeout aumentado de 20s para 40s**: Agora aguarda mais tempo para os anúncios carregarem
- **Seletores de anúncios atualizados**: Adicionados mais seletores alternativos para encontrar cards de anúncios
- **Melhor fallback para GraphQL**: Agora continua a execução se capturar anúncios via GraphQL mesmo que DOM não encontre

### Changed
- Atualizada versão para 2.1.0
- Melhorada espera antes de digitar no campo de busca
- Adicionado delay de 500-1000ms após limpar o input

### Added
- Mais seletores CSS para cards de anúncios:
  - `[data-testid="ad_card"]`
  - `div[class*="x1yztbdb"]`
  - `div[class*="ad-library-card"]`
  - `div[class*="_5m_f"]`
  - `div[class*="fbAdCard"]`

## [2.0.0] - 2024-12-01
- Versão inicial com anti-detection moderno e interceptação GraphQL
