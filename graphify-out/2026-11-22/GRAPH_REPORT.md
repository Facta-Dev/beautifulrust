# Graph Report - .  (2026-11-22)

## Corpus Check
- cluster-only mode — file stats not available

## Summary
- 1338 nodes · 1963 edges · 219 communities (175 shown, 44 thin omitted)
- Extraction: 97% EXTRACTED · 3% INFERRED · 0% AMBIGUOUS · INFERRED: 64 edges (avg confidence: 0.73)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `4c2e7404`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- server.ts
- Path
- CheckSkillTests
- lib.rs
- lib.rs
- lib.rs
- interface
- taskgraph.py
- HarnessTest
- banner.py
- check-examples.py
- What You Must Do When Invoked
- Beautiful Rust
- package.json
- Rust best practices
- config_parse
- Plan: a Beautiful Rust MCP server
- build-mcp-data.py
- Inventory
- Inventory
- compilerOptions
- Google Rust Style Guide (digest)
- Microsoft Pragmatic Rust Guidelines (digest)
- Rust review: <what was reviewed>
- Rust API Guidelines (digest)
- Changelog
- Rust port
- PackageTests
- graphify reference: extra exports and benchmark
- Rust Design Patterns (digest)
- Rust review: `inventory.rs`
- Effective Rust (digest)
- <app> API Designer
- <app> Migration Reviewer
- <app> Ownership Reviewer
- <app> Architect Agent
- <app> Build Resolver Agent
- <app> Code Explorer Agent
- <app> Code Reviewer Agent
- <app> Planner Agent
- <app> TDD Guide Agent
- <app> Unsafe Reviewer
- <app> Rust Test Author
- <app> Add Handler
- <app> Add Module
- <app> Claim Check skill
- <app> Clean-Room Rebuild skill
- <app> Corpus Retrieval skill
- <app> Diagnosing Bugs skill
- <app> Domain Modeling skill
- <app> Grilling skill
- <app> learn skill
- <app> Ownership Author
- <app> plan skill
- <app> Research skill
- <app> review skill
- <app> ship skill
- <app> spec skill
- <app> TDD skill
- <app> Unsafe Guard
- <app> Verified Status skill
- Cross-agent benchmark, October 2026
- graphify reference: query, path, explain
- Contributing
- Should fix
- Must fix
- vercel.json
- build
- README.md
- Bevy (digest)
- [1.2.0] - 2026-10-25
- [1.4.0] - 2026-10-26
- beautifulrust — agent instructions
- graphify reference: add a URL and watch a folder
- graphify reference: commit hook and native CLAUDE.md integration
- graphify reference: incremental update and cluster-only
- check-lints.sh
- guard-bash.sh
- /add-handler
- /add-module
- /claim-check
- /clean-room-rebuild
- /corpus-retrieval
- /diagnosing-bugs
- /domain-modeling
- /grilling
- /learn
- /ownership-author
- /plan
- /research
- /review
- /ship
- /spec
- /tdd
- /unsafe-guard
- /verified-status
- Playbooks for `beautifulrust` — load on demand
- graphify reference: GitHub clone and cross-repo merge
- graphify reference: transcribe video and audio
- Privacy policy
- blind.py
- CLAUDE.md
- README.md
- CREDITS.md
- CREDITS.md
- CREDITS.md
- CREDITS.md
- CREDITS.md
- extraction-spec.md
- CREDITS.md
- CREDITS.md
- CREDITS.md
- CREDITS.md
- mcp.json
- place-files.sh
- place-files.sh
- place-files.sh
- place-files.sh
- place-files.sh
- place-files.sh
- [1.5.0] - 2026-10-30

## God Nodes (most connected - your core abstractions)
1. `CheckSkillTests` - 44 edges
2. `build_valid_repo()` - 39 edges
3. `Checker` - 28 edges
4. `write()` - 25 edges
5. `Beautiful Rust` - 18 edges
6. `main()` - 16 edges
7. `YamlParser` - 16 edges
8. `interface` - 15 edges
9. `apply_hits()` - 15 edges
10. `Rust best practices` - 15 edges

## Surprising Connections (you probably didn't know these)
- `summarize()` --indirect_call--> `line()`  [INFERRED]
  mcp/src/crates.ts → mcp/test/crates.test.ts
- `enemies_in_range_hit_the_player()` --calls--> `Position`  [INFERRED]
  skills/rust-best-practices/evals/bevy-arena-regen/files/tests/arena.rs → skills/rust-best-practices/evals/bevy-arena-regen/files/src/lib.rs
- `enemies_in_range_hit_the_player()` --calls--> `Position`  [INFERRED]
  skills/rust-review/evals/review-bevy-arena/files/tests/arena.rs → skills/rust-review/evals/review-bevy-arena/files/src/lib.rs
- `connect()` --calls--> `createServer()`  [EXTRACTED]
  mcp/test/server.test.ts → mcp/src/server.ts
- `units_move_by_velocity_unless_stunned()` --calls--> `Position`  [INFERRED]
  skills/rust-best-practices/evals/bevy-arena-regen/files/tests/arena.rs → skills/rust-best-practices/evals/bevy-arena-regen/files/src/lib.rs

## Import Cycles
- None detected.

## Communities (219 total, 44 thin omitted)

### Community 0 - "server.ts"
Cohesion: 0.05
Nodes (58): CACHEABLE, CacheOptions, cachingFetcher(), Entry, compareSemver(), CrateAnswer, CrateLookupError, Fetcher (+50 more)

### Community 1 - "Path"
Cohesion: 0.11
Nodes (25): check_repo(), Checker, _fold_block(), format_problem(), _is_relative(), _json_key_line(), main(), _normalize_url() (+17 more)

### Community 2 - "CheckSkillTests"
Cohesion: 0.14
Nodes (12): add_mcp_plugin(), add_portable_plugin(), build_valid_repo(), CheckSkillTests, error_messages(), formatted(), load_checker(), png_header() (+4 more)

### Community 3 - "lib.rs"
Cohesion: 0.07
Nodes (47): Single, apply_hits(), ArenaConfig, ArenaPlugin, Armor, check_wave_cleared(), contact_damage(), damage_after_armor() (+39 more)

### Community 4 - "lib.rs"
Cohesion: 0.08
Nodes (45): apply_hits(), ArenaConfig, ArenaPlugin, Armor, check_wave_cleared(), contact_damage(), damage_after_armor(), Enemy (+37 more)

### Community 5 - "lib.rs"
Cohesion: 0.06
Nodes (26): Display, Error, Formatter, clone_text(), Flags, join_label(), Level, Mode (+18 more)

### Community 6 - "interface"
Cohesion: 0.06
Nodes (34): author, name, url, interface, publication, review, description, extensions (+26 more)

### Community 7 - "taskgraph.py"
Cohesion: 0.13
Nodes (19): CycleError, execution_order(), _find_cycle(), MissingDependency, parse_tasks(), ParseError, Exception, Parse a small task-definition format and compute a deterministic run order.  For (+11 more)

### Community 8 - "HarnessTest"
Cohesion: 0.11
Nodes (7): EndToEndTest, FindBlocksTest, HarnessTest, MappingTest, NormalizeTest, RepoTest, write()

### Community 9 - "banner.py"
Cohesion: 0.24
Nodes (27): add(), clamp(), compute_ground(), draw_text(), fbm(), gradient(), _h(), main() (+19 more)

### Community 10 - "check-examples.py"
Cohesion: 0.18
Nodes (26): apply_harness(), as_text(), Block, build_crate(), check_repo(), doc_files(), find_blocks(), first_code_line() (+18 more)

### Community 11 - "What You Must Do When Invoked"
Cohesion: 0.08
Nodes (24): For /graphify add and --watch, For /graphify query, For the commit hook and native CLAUDE.md integration, For --update and --cluster-only, /graphify, Honesty Rules, Interpreter guard for subcommands, Part A - Structural extraction for code files (+16 more)

### Community 12 - "Beautiful Rust"
Cohesion: 0.08
Nodes (25): Agent kit (Claude Code), Any agent, one command, Architecture diagrams, Beautiful Rust, Bevy, claude.ai, Claude Code, Contributing (+17 more)

### Community 13 - "package.json"
Cohesion: 0.08
Nodes (23): dependencies, @modelcontextprotocol/sdk, zod, description, devDependencies, esbuild, @types/node, typescript (+15 more)

### Community 14 - "Rust best practices"
Cohesion: 0.09
Nodes (22): 10. Documentation and comments, 11. Tests, 12. Performance, in order, 13. Final checklist, 1. Mindset, 2. Before you hand back code, 3. Ownership and borrowing, 4. Types and API design (+14 more)

### Community 15 - "config_parse"
Cohesion: 0.28
Nodes (19): config_t, config_count(), config_free(), config_get(), config_get_int(), config_parse(), dup_range(), fail() (+11 more)

### Community 16 - "Plan: a Beautiful Rust MCP server"
Cohesion: 0.11
Nodes (18): Build order, Claude Code, Code layout, Cost estimate, Decisions for you, Hosting, Hosting options, Phase 1: lookups, no code execution (+10 more)

### Community 17 - "build-mcp-data.py"
Cohesion: 0.22
Nodes (18): build_guidance(), build_lints(), explain(), github_slug(), main(), parse_lint_help(), parse_lints_toml(), Any (+10 more)

### Community 18 - "Inventory"
Cohesion: 0.27
Nodes (10): Inventory, InventoryError, Item, HashMap, Option, Rc, RefCell, Result (+2 more)

### Community 19 - "Inventory"
Cohesion: 0.27
Nodes (10): Inventory, InventoryError, Item, HashMap, Option, Rc, RefCell, Result (+2 more)

### Community 20 - "compilerOptions"
Cohesion: 0.12
Nodes (15): compilerOptions, allowImportingTsExtensions, erasableSyntaxOnly, lib, module, moduleResolution, noEmit, noUncheckedIndexedAccess (+7 more)

### Community 21 - "Google Rust Style Guide (digest)"
Cohesion: 0.12
Nodes (15): Background and goals, Code organization, Concurrency, Documentation, Formatting, Function inputs and outputs, Google Rust Style Guide (digest), Implementation concerns (+7 more)

### Community 22 - "Microsoft Pragmatic Rust Guidelines (digest)"
Cohesion: 0.13
Nodes (14): AI (agent-specific), Applications, Correctness, Documentation, FFI, Libraries: building, Libraries: interoperability, Libraries: resilience (+6 more)

### Community 23 - "Rust review: <what was reviewed>"
Cohesion: 0.13
Nodes (14): 1. Decide the scope, 1. <Short title> (`src/file.rs:42`), 2. ..., 2. Run the tools first, if you can, 3. ..., 3. What to look for, in priority order, 4. Write the report, 5. Offer the lints (+6 more)

### Community 24 - "Rust API Guidelines (digest)"
Cohesion: 0.15
Nodes (12): Debuggability, Dependability, Documentation, Flexibility, Future proofing, Interoperability, Macros, Naming (+4 more)

### Community 25 - "Changelog"
Cohesion: 0.25
Nodes (8): [1.0.0] - 2026-10-23, [1.1.0] - 2026-10-24, [1.3.0] - 2026-10-25, [1.6.0] - 2026-11-08, Added, Added, Changelog, [Unreleased]

### Community 26 - "Rust port"
Cohesion: 0.18
Nodes (10): 1. Understand the original before writing anything, 2. Port the tests first, 3. Design the Rust API, then implement it, 4. Keep the port proportionate, 5. Verify, 6. Write the porting notes, From C and C++, From Go, JavaScript, and TypeScript (+2 more)

### Community 28 - "graphify reference: extra exports and benchmark"
Cohesion: 0.22
Nodes (8): graphify reference: extra exports and benchmark, Step 6b - Wiki (only if --wiki flag), Step 7 - Neo4j export (only if --neo4j or --neo4j-push flag), Step 7a - FalkorDB export (only if --falkordb or --falkordb-push flag), Step 7b - SVG export (only if --svg flag), Step 7c - GraphML export (only if --graphml flag), Step 7d - MCP server (only if --mcp flag), Step 8 - Token reduction benchmark (only if total_words > 5000)

### Community 29 - "Rust Design Patterns (digest)"
Cohesion: 0.22
Nodes (8): Anti-patterns, Behavioural, Creational, Design patterns, Functional programming, Idioms, Rust Design Patterns (digest), Structural

### Community 30 - "Rust review: `inventory.rs`"
Cohesion: 0.25
Nodes (7): 11. Positional `bool` and look-alike `i64` parameters (`inventory.rs:42`, `:95`), 12. Missing standard traits on `Item` (`inventory.rs:15`), 13. String building with `+` and leftover clippy nits (`inventory.rs:46`, `:78`, `:79`, `:86`, `:98`, `:100`), Consider, Rust review: `inventory.rs`, Suggested lints, What's already good

### Community 31 - "Effective Rust (digest)"
Cohesion: 0.25
Nodes (7): Beyond standard Rust (Items 33-35), Concepts (Items 14-20), Dependencies (Items 21-26), Effective Rust (digest), Tooling (Items 27-32), Traits (Items 10-13), Types (Items 1-9)

### Community 32 - "<app> API Designer"
Cohesion: 0.29
Nodes (6): <app> API Designer, Core Mission, Expertise Areas, Guiding Principles, Output Format, Quality Standards

### Community 33 - "<app> Migration Reviewer"
Cohesion: 0.29
Nodes (6): <app> Migration Reviewer, Core Mission, Expertise Areas, Guiding Principles, Output Format, Quality Standards

### Community 34 - "<app> Ownership Reviewer"
Cohesion: 0.29
Nodes (6): <app> Ownership Reviewer, Core Mission, Expertise Areas, Guiding Principles, Output Format, Quality Standards

### Community 35 - "<app> Architect Agent"
Cohesion: 0.29
Nodes (6): <app> Architect Agent, Core Mission, Expertise Areas, Guiding Principles, Output Format, Quality Standards

### Community 36 - "<app> Build Resolver Agent"
Cohesion: 0.29
Nodes (6): <app> Build Resolver Agent, Core Mission, Expertise Areas, Guiding Principles, Output Format, Quality Standards

### Community 37 - "<app> Code Explorer Agent"
Cohesion: 0.29
Nodes (6): <app> Code Explorer Agent, Core Mission, Expertise Areas, Guiding Principles, Output Format, Quality Standards

### Community 38 - "<app> Code Reviewer Agent"
Cohesion: 0.29
Nodes (6): <app> Code Reviewer Agent, Core Mission, Expertise Areas, Guiding Principles, Output Format, Quality Standards

### Community 39 - "<app> Planner Agent"
Cohesion: 0.29
Nodes (6): <app> Planner Agent, Core Mission, Expertise Areas, Guiding Principles, Output Format, Quality Standards

### Community 40 - "<app> TDD Guide Agent"
Cohesion: 0.29
Nodes (6): <app> TDD Guide Agent, Core Mission, Expertise Areas, Guiding Principles, Output Format, Quality Standards

### Community 41 - "<app> Unsafe Reviewer"
Cohesion: 0.29
Nodes (6): <app> Unsafe Reviewer, Core Mission, Expertise Areas, Guiding Principles, Output Format, Quality Standards

### Community 42 - "<app> Rust Test Author"
Cohesion: 0.29
Nodes (6): <app> Rust Test Author, Core Mission, Expertise Areas, Guiding Principles, Output Format, Quality Standards

### Community 43 - "<app> Add Handler"
Cohesion: 0.29
Nodes (6): <app> Add Handler, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 44 - "<app> Add Module"
Cohesion: 0.29
Nodes (6): <app> Add Module, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 45 - "<app> Claim Check skill"
Cohesion: 0.29
Nodes (6): <app> Claim Check skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 46 - "<app> Clean-Room Rebuild skill"
Cohesion: 0.29
Nodes (6): <app> Clean-Room Rebuild skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 47 - "<app> Corpus Retrieval skill"
Cohesion: 0.29
Nodes (6): <app> Corpus Retrieval skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 48 - "<app> Diagnosing Bugs skill"
Cohesion: 0.29
Nodes (6): <app> Diagnosing Bugs skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 49 - "<app> Domain Modeling skill"
Cohesion: 0.29
Nodes (6): <app> Domain Modeling skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 50 - "<app> Grilling skill"
Cohesion: 0.29
Nodes (6): <app> Grilling skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 51 - "<app> learn skill"
Cohesion: 0.29
Nodes (6): <app> learn skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 52 - "<app> Ownership Author"
Cohesion: 0.29
Nodes (6): <app> Ownership Author, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 53 - "<app> plan skill"
Cohesion: 0.29
Nodes (6): <app> plan skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 54 - "<app> Research skill"
Cohesion: 0.29
Nodes (6): <app> Research skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 55 - "<app> review skill"
Cohesion: 0.29
Nodes (6): <app> review skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 56 - "<app> ship skill"
Cohesion: 0.29
Nodes (6): <app> ship skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 57 - "<app> spec skill"
Cohesion: 0.29
Nodes (6): <app> spec skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 58 - "<app> TDD skill"
Cohesion: 0.29
Nodes (6): <app> TDD skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 59 - "<app> Unsafe Guard"
Cohesion: 0.29
Nodes (6): <app> Unsafe Guard, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 60 - "<app> Verified Status skill"
Cohesion: 0.29
Nodes (6): <app> Verified Status skill, Core Principles, Output Format, Research References, Rules, When to Activate

### Community 61 - "Cross-agent benchmark, October 2026"
Cohesion: 0.33
Nodes (5): Caveats, Cross-agent benchmark, October 2026, How it was run, One regression, Results

### Community 62 - "graphify reference: query, path, explain"
Cohesion: 0.33
Nodes (5): For /graphify explain, For /graphify path, graphify reference: query, path, explain, Step 0 — Constrained query expansion (REQUIRED before traversal), Step 1 — Traversal

### Community 63 - "Contributing"
Cohesion: 0.33
Nodes (6): Contributing, Good first contributions, License, Making a change, Style, The one rule: every rule needs a source

### Community 64 - "Should fix"
Cohesion: 0.33
Nodes (6): 10. No tests and no docs (whole file), 6. Double lookups, check-then-unwrap, and clone-to-mutate (`inventory.rs:35-36`, `:61-64`), 7. `#![deny(warnings)]` already breaks `cargo clippy` (`inventory.rs:1`), 8. `&String` and `&Vec<T>` parameters (`inventory.rs:34`, `:51`, `:60`, `:71`, `:82`), 9. `report` output order is random (`inventory.rs:97`), Should fix

### Community 65 - "Must fix"
Cohesion: 0.33
Nodes (6): 1. Loading a file panics on bad input (`inventory.rs:76`, `:77`, `:83`), 2. `total_value` panics on an unknown name, and the arithmetic can overflow (`inventory.rs:54`, `:55`, `:63`), 3. The "no negative quantity or price" rule is only enforced in one of four places (`inventory.rs:17-20`, `:43`, `:63`, `:71-79`), 4. The error type gives callers nothing to act on (`inventory.rs:6-13`), 5. `Rc<RefCell<...>>` in the public API, twice (`inventory.rs:24`, `:28`, `:82`), Must fix

### Community 66 - "vercel.json"
Cohesion: 0.33
Nodes (5): buildCommand, framework, outputDirectory, rewrites, $schema

### Community 67 - "build"
Cohesion: 0.53
Nodes (5): build(), main(), package_files(), Path, Files to package, relative to root, in a stable order.

### Community 69 - "Bevy (digest)"
Cohesion: 0.40
Nodes (4): Bevy (digest), Correctness checks, Keep Bevy's conventions, Testing systems

### Community 70 - "[1.2.0] - 2026-10-25"
Cohesion: 0.50
Nodes (4): [1.2.0] - 2026-10-25, Added, Changed, Verified

### Community 71 - "[1.4.0] - 2026-10-26"
Cohesion: 0.50
Nodes (4): [1.4.0] - 2026-10-26, Added, Changed, Fixed

### Community 72 - "beautifulrust — agent instructions"
Cohesion: 0.50
Nodes (3): beautifulrust — agent instructions, graphify, Model routing (Claude Code + Ollama)

### Community 73 - "graphify reference: add a URL and watch a folder"
Cohesion: 0.50
Nodes (3): For /graphify add, For --watch, graphify reference: add a URL and watch a folder

### Community 74 - "graphify reference: commit hook and native CLAUDE.md integration"
Cohesion: 0.50
Nodes (3): For git commit hook, For native CLAUDE.md integration, graphify reference: commit hook and native CLAUDE.md integration

### Community 75 - "graphify reference: incremental update and cluster-only"
Cohesion: 0.50
Nodes (3): For --cluster-only, For --update (incremental re-extraction), graphify reference: incremental update and cluster-only

### Community 76 - "check-lints.sh"
Cohesion: 0.50
Nodes (3): CARGO_TERM_COLOR, CLIPPY_CONF_DIR, check-lints.sh script

### Community 77 - "guard-bash.sh"
Cohesion: 0.83
Nodes (3): has(), has_i(), guard-bash.sh script

### Community 218 - "[1.5.0] - 2026-10-30"
Cohesion: 0.50
Nodes (4): [1.5.0] - 2026-10-30, Added, Changed, Fixed

## Knowledge Gaps
- **482 isolated node(s):** `Silent`, `Flags`, `Mode`, `Level`, `beautiful-rust` (+477 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **44 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `render()` connect `check-examples.py` to `Path`?**
  _High betweenness centrality (0.002) - this node is a cross-community bridge._
- **Why does `Changelog` connect `Changelog` to `[1.5.0] - 2026-10-30`, `README.md`, `[1.2.0] - 2026-10-25`, `[1.4.0] - 2026-10-26`?**
  _High betweenness centrality (0.001) - this node is a cross-community bridge._
- **Why does `Rust review: `inventory.rs`` connect `Rust review: `inventory.rs`` to `Should fix`, `Must fix`?**
  _High betweenness centrality (0.001) - this node is a cross-community bridge._
- **What connects `Render a square icon by re-pointing the scene globals at a small canvas.`, `Copy each run into grading/<case>/run-N without skills, git, or build output, an`, `Silent` to the rest of the system?**
  _503 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `server.ts` be split into smaller, more focused modules?**
  _Cohesion score 0.052982456140350874 - nodes in this community are weakly interconnected._
- **Should `Path` be split into smaller, more focused modules?**
  _Cohesion score 0.10536130536130536 - nodes in this community are weakly interconnected._
- **Should `CheckSkillTests` be split into smaller, more focused modules?**
  _Cohesion score 0.13721804511278196 - nodes in this community are weakly interconnected._