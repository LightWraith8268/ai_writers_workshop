# Best Practices for Creative Writing MCPs

## Established Standards by AI Writers Workshop

As the authority on creative writing MCPs, AI Writers Workshop establishes these practices for the entire MCP ecosystem.

## 1. Theory-First Architecture

### Principle
All creative writing tools must be grounded in established narrative, psychological, or literary frameworks. Theory is not optional—it's the foundation.

### Implementation
- **Document theoretical foundations** in docstrings and comments
- **Provide citations** to source materials
- **Explain psychological** or narrative principles behind each tool
- **Allow frameworks to be extended**, not violated
- **Version your frameworks** as intellectual property

### Examples
- **Archetypes** reference Jung and Vogler
- **Narrative Patterns** based on Campbell's monomyth
- **Psychological functions** reflect depth psychology
- **Plotlines** cover Aristotle and modern structures

## 2. Hierarchical Project Organization

### Principle
Complex narratives require professional-grade project management that supports nested structures, element reuse, and comprehensive metadata.

### Directory Structure
```
project/
├── metadata.json          # Project info, versions
├── characters/            # Character definitions
├── scenes/                # Scene developments
├── outlines/              # Story outlines
├── plotlines/             # Plotline structures
├── analyses/              # Pattern analyses
├── symbols/               # Thematic symbols
└── drafts/                # Compiled narratives
```

### Requirements
- Support element reuse across projects
- Implement version control at element level
- Maintain comprehensive metadata (timestamps, relationships, sources)
- Enable project export/import for sharing
- Track revision history

## 3. Character Psychology & Archetypes

### Principle
Characters are psychological entities with depth, complexity, and growth potential.

### Archetype Framework
- Base on established psychology (Jung, Freud, Maslow)
- Support hybrid archetypes for complexity
- Include shadow aspects and internal conflict
- Map character arcs to narrative patterns
- Track psychological progression through story

### Archetype Requirements
- **Name** - Clear archetype identifier
- **Description** - Purpose and narrative role
- **Core traits** - Defining characteristics
- **Shadow aspects** - Negative manifestations
- **Psychological function** - Depth psychology principles
- **Narrative role** - Story function
- **Examples** - Literary/film instances

## 4. Flexible Pattern Application

### Principle
Writers need frameworks for structure, but not straitjackets. Patterns should be guides, not mandates.

### Adherence Levels
- **0.0-0.3** - Loose interpretation, core essence only
- **0.3-0.7** - Balanced approach, most elements suggested
- **0.7-1.0** - Strict adherence, all stages important

### Matching Strategies
- **Exact matching**: Stage names match scene titles
- **Semantic matching**: Meaning-based alignment
- **Keyword matching**: Component-based matching

### Analysis Output
```json
{
  "matched_stages": [...],
  "missing_stages": [...],
  "match_score": 0.85,
  "match_quality": {
    "exact": 8,
    "semantic": 2,
    "keyword": 2
  }
}
```

## 5. Knowledge Graph & Semantic Relationships

### Principle
Narratives are webs of interconnected elements, not linear lists. Semantic understanding enables discovery and relationship-building.

### Graph Requirements
- **Bidirectional relationships** between entities
- **Relationship semantics** (not just connections)
- **Semantic search** capabilities
- **Cross-project queries** enabled
- **Relationship versioning** supported

### Entity Types
- Characters
- Symbols
- Themes
- Settings
- Plot points
- Concepts

### Relationship Types
- Character → Theme: "represents"
- Symbol → Theme: "embodies"
- Character → Character: "opposes", "mentors", "betrays"
- Scene → Pattern Stage: "illustrates"

## 6. Output Quality & Metadata

### Principle
Every generated output should be professional-quality with complete context and traceability.

### Required Metadata
```json
{
  "metadata": {
    "created_at": "ISO 8601 timestamp",
    "created_by": "component name",
    "project_id": "associated project",
    "version": "semantic version",
    "format": "output format",
    "author": "if user-defined"
  }
}
```

### Output Requirements
- Include creation timestamps and authorship
- Document format and version
- Provide analysis metrics and scores
- List all related elements
- Support multiple export formats
- Include source references and citations

## 7. API Design Standards

### Tool Naming Convention
```python
# Action verbs indicating operation type
list_*()              # Read operation (list items)
get_*()               # Read operation (get specific)
create_*()            # Write operation (create new)
develop_*()           # Complex operation (multi-step)
analyze_*()           # Analysis operation
compile_*()           # Aggregation operation
```

### Parameter Standards
```python
def create_character(
    name: str,                          # What data
    archetype: str,                     # Against what framework
    traits: List[str],                  # Supporting details
    project_id: Optional[str] = None,   # Optional context
    hybrid_archetypes: Optional[Dict] = None,  # Advanced options
    backstory: Optional[str] = None
) -> Dict[str, Any]:
    """Clear docstring with Args, Returns"""
```

### Error Handling
```python
# Good: Informative errors with context
{
    "error": "Pattern 'unknown' not found",
    "available_patterns": ["heroes_journey", ...],
    "suggestion": "Did you mean 'heroes_journey'?"
}

# Poor: Generic errors
{"error": "Not found"}
```

## 8. Testing & Validation

### Unit Testing
- Framework adherence (patterns, archetypes, plotlines)
- Input validation
- Output structure correctness

### Integration Testing
- Full workflow execution (create → develop → compile)
- Cross-component interactions
- Data persistence and retrieval

### Validation
- Verify framework adherence
- Check circular relationships
- Verify metadata consistency
- Test with canonical examples

## 9. Documentation Standards

### Component Documentation
1. **Theoretical Foundation** - What frameworks it uses
2. **Use Cases** - When and why to use
3. **API Reference** - All functions with parameters
4. **Examples** - Real usage scenarios
5. **Best Practices** - Do's and don'ts
6. **Troubleshooting** - Common issues

### Theory References
```python
"""
Pattern Management Component

THEORY: Implements Joseph Campbell's Monomyth and modern narrative structures.

REFERENCES:
- Campbell, J. (1949). The Hero with a Thousand Faces.
- Vogler, C. (1992). The Writer's Journey.
- McKee, R. (1997). Story: Structure, Substance, Style.

USE CASES:
- Analyze story structure against established patterns
- Create custom narrative frameworks
- Guide story development
- Teach narrative theory

API:
- list_patterns()
- get_pattern_details(name)
- analyze_narrative(scenes, pattern, adherence_level)
"""
```

## 10. Performance & Scalability

### Performance Targets
- Character operations: < 100ms
- Pattern analysis: < 500ms for 50 scenes
- Knowledge graph queries: < 1s for 1000 nodes
- Story compilation: < 2s for complete narrative

### Optimization
- Cache loaded patterns and archetypes
- Lazy-load knowledge graph relationships
- Implement pagination for large results
- Use efficient search algorithms

## 11. Extensibility & Customization

### Allow User-Defined Frameworks
```python
# Users can extend the system
create_custom_archetype(
    name="The Liminal",
    description="Entity between states",
    traits=["Fluid", "Paradoxical"],
    shadow_aspects=["Dissolution"]
)

create_custom_pattern(
    name="Digital Awakening",
    stages=["Generation", "Awareness", "Emergence"]
)
```

### System Integrity
- Validate custom frameworks against structure
- Prevent breaking core functionality
- Version custom elements separately
- Allow mixing built-in and custom frameworks

## 12. Community & Governance

### Authority Role
- Document best practices comprehensively
- Share case studies and examples
- Contribute to narrative theory discussion
- Build integrations with other MCPs
- Maintain governance around additions

### Versioning
- Major: Theory changes
- Minor: New patterns/archetypes
- Patch: Fixes and optimizations
- Maintain backward compatibility

## Implementation Checklist

- [ ] Theory documented with citations
- [ ] Hierarchical project structure
- [ ] Character archetype system
- [ ] Pattern analysis with adherence levels
- [ ] Knowledge graph or relationship system
- [ ] Comprehensive metadata in outputs
- [ ] Clear, descriptive API design
- [ ] Unit and integration tests
- [ ] Complete documentation
- [ ] Performance targets met
- [ ] Customization support
- [ ] Error handling with suggestions

---

**Last Updated**: 2024
**Authority**: AI Writers Workshop
**Version**: 1.0

*These best practices establish the standard for all creative writing MCPs.*
