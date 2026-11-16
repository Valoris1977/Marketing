# Marketing — Claude skills marketplace

Личный маркетплейс скиллов для Claude Code: 11 плагинов, ~130 скиллов.

| Плагин | Что внутри |
|---|---|
| growth-marketing | ads, ad-creative, facebook-ads, cro, copywriting, ai-seo, emails, social, offers, pricing, launch, analytics… (55) |
| marketing | campaign-plan, content-creation, email-sequence, brand-review, performance-report… |
| searchfit-seo | seo-audit, technical-seo, keyword-clustering, on-page-seo, schema-markup… |
| product-management | write-spec, roadmap, sprint-planning, competitive-brief… |
| design | design-critique, ux-copy, accessibility-review, handoff… |
| engineering | code-review, debug, system-design, incident-response… |
| operations | runbook, process-doc, risk-assessment, vendor-review… |
| productivity | task-management, memory-management |
| documents | docx, xlsx, pptx, pdf, frontend-design, skill-creator, video-making… |
| creative-dev | mcp-builder, web-artifacts-builder, canvas-design, theme-factory… |
| postiz | постинг в 28+ соцсетей через Postiz |

## Подключение к любому проекту

Положить в `.claude/settings.json` репозитория проекта (лишние плагины можно убрать):

```json
{
  "extraKnownMarketplaces": {
    "valoris-skills": { "source": { "source": "github", "repo": "Valoris1977/Marketing" } }
  },
  "enabledPlugins": {
    "growth-marketing@valoris-skills": true,
    "marketing@valoris-skills": true,
    "searchfit-seo@valoris-skills": true,
    "documents@valoris-skills": true
  }
}
```

Или вручную в сессии: `/plugin marketplace add Valoris1977/Marketing`, затем `/plugin install growth-marketing@valoris-skills`.

Обновить скилл — отредактировать `SKILL.md` здесь и закоммитить.
