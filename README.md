# Claude Plugins Marketplace

Personal Claude Code plugin marketplace by Chris Prather.

## Plugins

### crochet

Intelligence layer for [git-zhi](https://github.com/perigrin/git-zhi).
Skills for decomposing specs into executable dependency chains, importing
external tickets, generating narrative reports, onboarding repos, and
validating pipeline outputs.

| Skill | Purpose |
|-------|---------|
| `crochet:refinement` | Decompose a spec into an executable git-zhi chain |
| `crochet:assess` | Gap analysis: PRD vs codebase |
| `crochet:import` | Assisted ticket import from Jira with dependency inference |
| `crochet:report` | Narrative reports from templates with Mermaid charts |
| `crochet:onboard` | Step-by-step git-zhi adoption walkthrough |
| `crochet:pushback` | Pre-flight validation of specs, historian output, report templates |
| `crochet:alignment` | Post-pipeline verification: refinement vs PRD, historian vs git log |
| `crochet:postmortem` | Mandatory process retrospective at milestone completion |
| `crochet:install` | Install the git-zhi binary and companion symlinks |

Requires [git-zhi](https://github.com/perigrin/git-zhi) on `$PATH`. Run
`crochet:install` to set it up automatically.

### perl-development

Agentic Perl development — version-aware code generation, Test2 testing,
dependency management, static analysis, and regression testing across the
production version matrix. PVM is the reference backend; alternative
backends are a community contribution path.

| Skill | Purpose |
|-------|---------|
| `perl:setup` | Select backend, scaffold project |
| `perl:write-perl` | Version-detecting code generation (dispatches to 5.42/5.40/5.38/5.36/toolchain) |
| `perl:test-perl` | Test2::V0 testing with TDD workflow |
| `perl:test-mojolicious` | Test::Mojo for Mojolicious apps |
| `perl:debug-perl` | Systematic debugging with psc and pvx |
| `perl:manage-deps` | CPAN dependency management via cpanfile |
| `perl:review-perl` | Static analysis with perlcritic and perltidy |
| `perl:regression-test` | Version matrix testing via PVM binary cache |

### commonplacebook

Semantic search and journaling for zk notebooks. Adds keyword, semantic,
and similar-note search plus a daily journal interview command.

## Installation

Add this marketplace to Claude Code:

```
/plugin marketplace add perigrin/claude-plugins-marketplace
```

Then install plugins:

```
/plugin install crochet
/plugin install perl-development
/plugin install commonplacebook
```
