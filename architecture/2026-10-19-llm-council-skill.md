# LLM Council (skill Claude Code)

- **Date :** 2026-10-19
- **Lien d'origine :** vidéo TikTok @unefille.ia — https://vt.tiktok.com/ZSgrdayRF/
- **Dépôt :** https://github.com/tenfoldmarc/llm-council-skill (dernier commit : 18/04/2026)
- **Type :** skill Claude Code (un seul fichier `SKILL.md`, aucun code exécutable)
- **Demande :** vérifier ce que présente la vidéo (« Claude est trop d'accord avec vous »)

## Ce que c'est
Un texte d'instructions pour Claude Code, adapté du « LLM Council » d'Andrej Karpathy.
Une question est soumise à 5 sous-agents qui ont chacun un rôle :
- le **Contradicteur**, qui cherche ce qui va échouer ;
- le **Penseur des premiers principes**, qui vérifie qu'on se pose la bonne question ;
- l'**Expansionniste**, qui cherche le potentiel caché ;
- l'**Œil extérieur**, qui n'a aucun contexte ;
- l'**Exécutant**, qui demande « que fait-on lundi matin ? ».

Ensuite, chacun relit les 5 réponses de façon anonyme. Un « président » fait la synthèse :
points d'accord, points de désaccord, angles morts, recommandation et une première action.
Le résultat est un rapport HTML et une transcription en Markdown.

## Comment l'installer
```sh
git clone https://github.com/tenfoldmarc/llm-council-skill ~/.claude/skills/llm-council
# ou, pour ce dépôt seulement : copier SKILL.md dans .claude/skills/llm-council/
```
Pour le lancer, écrire « council this : <question> », « stress-test this », etc.

## Ce qui a été vérifié
| Vérification | Résultat |
|---|---|
| Lien TikTok résolu, description lue (oEmbed) | ✅ correspond au dépôt |
| Contenu du dépôt | ✅ seulement SKILL.md, README et .gitignore : pas de script ni d'accès réseau, inoffensif |
| Format du skill (frontmatter name/description) | ✅ valide pour Claude Code |
| Exécution réelle d'un conseil | ⏸ non lancée (11 agents par conseil, coûteux en quota) |

## Verdict
Sérieux et utile pour les **vraies décisions** (prix, choix entre deux options, lancement d'un projet).
Inutile pour des questions simples. Points d'attention :
- coût d'environ 11 sous-agents par conseil, ce qui consomme vite le quota hebdomadaire ;
- les 5 « conseillers » sont le même modèle avec des rôles différents. Pour une vraie diversité de modèles, voir `karpathy/llm-council` (GPT, Gemini, Grok…, avec des clés API payantes).

## Suites possibles
- L'installer dans ce dépôt (`.claude/skills/llm-council/`) et le tester sur une vraie question, par exemple l'offre de sites web pour les restos de Yaoundé.
