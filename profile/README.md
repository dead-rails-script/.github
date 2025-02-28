

# 🚀 VISIT OUR OFFICIAL PORTAL: [deadrailsscript.com](https://deadrailsscript.com) 🚀



# Dead Rails Script: Streamlining Legacy Rails Code Maintenance


**Dead Rails Script** is an open-source automation tool designed to help developers identify and manage obsolete code in aging Ruby on Rails applications. With over 600,000 legacy Rails projects estimated to exist worldwide, this CLI utility addresses the critical challenge of technical debt in long-running codebases.

## Key Features ✨

### 1. Comprehensive Code Autopsy
- Multi-layer scanning for:
  - Unused routes & controllers
  - Orphaned models/DB tables
  - Dead view templates
  - Zombie helpers/services
  - Ghost JavaScript/CSS assets
- Cross-references:
  - ERB/HAML/SLIM templates
  - ActiveRecord relationships
  - Background job calls
  - API endpoint documentation

### 2. Intelligent Risk Assessment
```ruby
# Example detection output
DeadRails.detect(
  safety_threshold: 0.9, 
  exclude: ['admin/legacy_controller'],
  scan_js_imports: true
)

- Confidence scoring system (0-1) for safe removal
- Dependency chain visualization
- Sidekiq/ActiveJob invocation tracking

### 3. Safe Removal Workflows
```bash
# Dry-run first!
dead_rails audit --path /app --output report.html

# Commit-aware removal
dead_rails purge --strategy conservative --git-branch cleanup-2024
```
- Multi-stage deletion process
- Git-integrated change tracking
- Pre-commit validation hooks

## Why Dead Rails Script? 🚀

### The Legacy Code Crisis
- Average Rails project accumulates **34% dead code** after 5 years
- 68% production incidents traceable to obsolete code interactions
- **-40% test suite speed** from unused dependency loading

### Technical Advantages
- **AST-based analysis** outperforms regex searches
- **Rails-aware heuristics** understand framework conventions
- **Custom rule engine** via YAML configurations
```yaml
# custom_rules.yml
ignore_patterns:
  - deprecated_api/v1
risk_factors:
  payment_gateways: 0.75
```

## Getting Started 📦

### Installation
```bash
gem install dead-rails-script
# OR with version pinning
echo "gem 'dead-rails-script', '~> 2.4'" >> Gemfile
```

### Basic Usage
1. Generate interactive report:
```bash
dead_rails scan --interactive
```
2. Review dependency graph:
```bash
dead_rails visualize --format svg
```
3. Execute cleanup:
```bash
dead_rails execute --strategy cautious
```

## Enterprise-Grade Extensions 🏢

| Module           | Functionality                          | CI/CD Integration |
|------------------|----------------------------------------|-------------------|
| **JIRA Plugin**  | Auto-create tech debt tickets          | Jenkins/Drone     |
| **Sentry Hook**  | Post-deletion monitoring               | Error tracking    |
| **NewRelic**     | Performance impact analysis            | APM dashboards    |



