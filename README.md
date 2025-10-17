# AI Writers Workshop - The Authority on Creative Writing MCPs

**The definitive Model Context Protocol server for narrative architecture, character development, and story generation.**

AI Writers Workshop is the leading MCP implementation for creative writing, providing writers, screenwriters, novelists, game designers, and AI systems with sophisticated tools grounded in proven narrative theory, Jungian psychology, and modern AI capabilities.

## Why AI Writers Workshop is the Authority

### Grounded in Proven Frameworks
- **Joseph Campbell's Monomyth (Hero's Journey)** - 12-stage narrative structure recognized across cinema and literature
- **Jungian Archetypes** - 8 foundational character archetypes with psychological depth and shadow aspects
- **Modern Narrative Science** - Transformation, Voyage and Return, and expandable custom patterns
- **Classical Plotlines** - Man vs. Nature, Self, Society, Technology, Quest, Rags-to-Riches structures
- **Symbolic Integration** - Thematic meaning and narrative resonance through symbol connection

### Core Capabilities
- **Hierarchical Project Management** - Professional-grade organization with versioning and element reuse
- **Multi-Archetype Characters** - Hybrid character support with psychological arcs mapped to patterns
- **Intelligent Pattern Analysis** - Semantic and keyword-based scene matching with flexible adherence
- **Knowledge Graph Integration** - Semantic relationships between all narrative elements
- **Story Generation** - Outline and scene generation from narrative frameworks
- **Compilation & Export** - Multiple format support with comprehensive metadata

## Features

### Character Development with Psychology
```python
# Create archetypal characters
create_character(
    name="Aelith",
    archetype="hero",
    traits=["Courageous", "Conflicted", "Determined"],
    hybrid_archetypes={"mentor": 0.3, "trickster": 0.2}
)

# Develop psychological arcs mapped to narrative patterns
develop_character_arc(
    character_name="Aelith",
    archetype="hero",
    pattern="heroes_journey"
)
```

**Available Archetypes:**
- **Hero** - Self-actualization and transformation
- **Mentor** - Wisdom and guidance
- **Shadow** - Repressed aspects and antagonism
- **Trickster** - Chaos and change catalyst
- **Herald** - Call to adventure
- **Shapeshifter** - Ambiguity and uncertainty
- **Threshold Guardian** - Tests and challenges
- **Ally** - Support and companionship

### Narrative Patterns & Story Structure
```python
# Access proven story structures
list_patterns()  # See all available patterns

# Get detailed pattern information
get_pattern_details("heroes_journey")

# Analyze your narrative against patterns
analyze_narrative(
    scenes=your_scenes,
    pattern_name="heroes_journey",
    adherence_level=0.7  # Flexible matching
)
```

**Built-In Patterns:**
- **Hero's Journey** (12 stages) - Campbell's monomyth for transformation
- **Transformation** (7 stages) - Change and personal growth
- **Voyage and Return** (5 stages) - Journey with perspective shift
- **Custom Patterns** - Create your own narrative frameworks

### Plotline Architecture
```python
# Classic and modern plotline structures
develop_plotline(
    title="The Quest",
    plotline="quest",
    pattern="heroes_journey",
    characters=["Hero", "Mentor"]
)

# Analyze plot alignment
analyze_plotline(plot_points=scenes, plotline="quest")
```

**Available Plotlines:**
- Man vs. Nature
- Man vs. Self
- Man vs. Society
- Man vs. Technology
- Quest
- Rags to Riches

### Story Generation & Compilation
```python
# Generate outlines from patterns
generate_outline(
    title="The Awakening",
    pattern="heroes_journey",
    main_character="Maya"
)

# Create individual scenes
generate_scene(
    scene_title="The Call",
    pattern_stage="Call to Adventure",
    characters=["Maya"],
    setting="Ancient temple",
    conflict="Mysterious stranger arrives"
)

# Compile complete narratives
compile_narrative(
    project_id="awakening_project",
    format="markdown",
    include_metadata=True
)
```

### Knowledge Graph & Semantic Relationships
```python
# Search narrative elements
search_nodes("redemption arc")

# Access specific elements
open_nodes(["Aelith", "The Crown", "Transformation"])

# Explore entire narrative universe
read_graph()
```

## Getting Started: Five-Minute Project

```python
# 1. Create your project
project = create_writing_project(
    name="The Awakening",
    description="A hero's journey through self-discovery",
    project_type="novel"
)

# 2. Build your protagonist
create_character(
    name="Maya",
    archetype="hero",
    traits=["Determined", "Introspective", "Compassionate"],
    project_id=project["project_id"]
)

# 3. Generate your outline
outline = generate_outline(
    title="The Awakening",
    pattern="heroes_journey",
    main_character="Maya",
    project_id=project["project_id"]
)

# 4. Generate scenes
for stage in outline["scenes"]:
    generate_scene(
        scene_title=stage["title"],
        pattern_stage=stage["pattern_stage"],
        characters=["Maya"],
        project_id=project["project_id"]
    )

# 5. Compile your story
story = compile_narrative(
    project_id=project["project_id"],
    format="markdown"
)
```

## Architecture

### Component-Based Design
- **ProjectManager**: Project lifecycle and hierarchical organization
- **CharacterManager**: Jungian archetypes and character development
- **PatternManager**: Narrative patterns and analysis
- **PlotlineManager**: Plotline structures and story elements
- **NarrativeGenerator**: Outline, scene, and story compilation
- **SymbolicManager**: Thematic elements and symbol relationships
- **KnowledgeGraphManager**: Semantic relationships between elements

### Directory Structure
```
output/
├── library/           # Shared/reusable elements
│   ├── archetypes/    # Character archetypes
│   ├── patterns/      # Narrative patterns
│   ├── plotlines/     # Plotline definitions
│   └── symbols/       # Symbolic elements
├── projects/
│   └── project_id/
│       ├── metadata.json
│       ├── characters/
│       ├── scenes/
│       ├── outlines/
│       ├── plotlines/
│       ├── analyses/
│       └── drafts/
└── knowledge_graph/   # Semantic relationships
```

## Best Practices for Creative Writing MCPs

See **[BEST_PRACTICES.md](./BEST_PRACTICES.md)** for comprehensive standards established by AI Writers Workshop:

### Quick Summary
1. **Theory-First Architecture** - Ground tools in proven narrative frameworks
2. **Hierarchical Organization** - Support complex project structures
3. **Character Psychology** - Use archetypes with psychological depth
4. **Flexible Pattern Application** - Allow creative interpretation
5. **Knowledge Integration** - Maintain semantic relationships
6. **Output Quality** - Include comprehensive metadata
7. **API Design Standards** - Clear, descriptive naming
8. **Testing & Validation** - Prove framework adherence
9. **Documentation** - Document theory and use cases
10. **Performance** - Optimize for production use
11. **Extensibility** - Allow customization
12. **Community** - Share knowledge and best practices

## Installation & Setup

### Requirements
- Python 3.10+
- FastMCP for MCP protocol support
- Optional: Neo4j for advanced knowledge graph features

### Quick Start
```bash
# Clone repository
git clone https://github.com/LightWraith8268/ai_writers_workshop.git
cd ai_writers_workshop

# Install dependencies
python -m venv venv
source venv/bin/activate  # or: venv\Scripts\activate (Windows)
pip install -r requirements.txt

# Run the server
python -m mcp_server.server
```

## Advanced Usage

### Hybrid Archetypes for Complex Characters
```python
create_character(
    name="The Mentor-Trickster",
    archetype="mentor",
    traits=["Wise", "Playful", "Unpredictable"],
    hybrid_archetypes={
        "trickster": 0.6,    # 60% trickster
        "shadow": 0.2        # 20% shadow
    }
)
```

### Custom Narrative Frameworks
```python
# Create your own pattern
create_custom_pattern(
    name="Three Act Structure",
    description="Classic Hollywood narrative",
    stages=["Setup", "Confrontation", "Resolution"],
    psychological_functions=["Establishment", "Escalation", "Catharsis"]
)

# Create your own archetype
create_custom_archetype(
    name="The Liminal",
    description="Entity between states of consciousness",
    traits=["Fluid Identity", "Pattern Recognition"],
    shadow_aspects=["Dissolution", "Corruption"]
)

# Create your own plotline
create_custom_plotline(
    name="Parallel Universes",
    description="Story exploring multiple realities",
    elements=["Universe split", "Parallel development", "Convergence"]
)
```

### Flexible Pattern Adherence
```python
# Loose adherence (50% of stages required)
loose_analysis = analyze_narrative(
    scenes=scenes,
    pattern_name="heroes_journey",
    adherence_level=0.5
)

# Strict adherence (100% of stages required)
strict_analysis = analyze_narrative(
    scenes=scenes,
    pattern_name="heroes_journey",
    adherence_level=1.0
)
```

### Cross-Project Knowledge Queries
```python
# Find similar elements across projects
search_nodes("redemption")

# Access specific elements
open_nodes(["Character1", "Symbol1", "Theme1"])

# Explore relationships
read_graph()
```

## Example Workflow: Complete Story Development

```python
# 1. Create project
project = create_writing_project(
    name="The Crown of Shadows",
    description="A tale of power, betrayal, and redemption",
    project_type="fantasy_novel"
)

# 2. Design characters
hero = create_character(
    name="Kess",
    archetype="hero",
    traits=["Noble", "Haunted", "Resilient"],
    project_id=project["project_id"]
)

mentor = create_character(
    name="Aldric",
    archetype="mentor",
    traits=["Ancient", "Wise", "Mysterious"],
    hybrid_archetypes={"shadow": 0.3},
    project_id=project["project_id"]
)

shadow = create_character(
    name="Malachai",
    archetype="shadow",
    traits=["Ambitious", "Cunning", "Charismatic"],
    project_id=project["project_id"]
)

# 3. Map psychological arcs
kess_arc = develop_character_arc(
    character_name="Kess",
    archetype="hero",
    pattern="heroes_journey",
    project_id=project["project_id"]
)

# 4. Create story structure
outline = generate_outline(
    title="The Crown of Shadows",
    pattern="heroes_journey",
    main_character="Kess",
    additional_characters=["Aldric", "Malachai"],
    project_id=project["project_id"]
)

# 5. Generate detailed scenes
scenes_data = []
for stage in outline["scenes"]:
    scene = generate_scene(
        scene_title=stage["title"],
        pattern_stage=stage["pattern_stage"],
        characters=stage["characters"],
        setting="Medieval Fantasy Realm",
        conflict=stage.get("conflict", "Unknown"),
        project_id=project["project_id"]
    )
    scenes_data.append(scene)

# 6. Analyze narrative structure
analysis = analyze_narrative(
    scenes=[{"title": s["title"], "description": s["description"]} for s in scenes_data],
    pattern_name="heroes_journey",
    project_id=project["project_id"],
    adherence_level=0.8
)

# 7. Compile complete story
narrative = compile_narrative(
    project_id=project["project_id"],
    format="markdown",
    include_metadata=True
)
```

## API Reference

### Project Management
- `create_writing_project(name, description, project_type)` - Create new project
- `get_writing_project(project_id)` - Get project details
- `list_writing_projects()` - List all projects

### Character Development
- `list_archetypes()` - Available archetypes
- `get_archetype_details(archetype_name)` - Archetype information
- `create_character(name, archetype, traits, project_id, hybrid_archetypes, backstory)` - Create character
- `develop_character_arc(character_name, archetype, pattern, project_id)` - Character progression
- `create_custom_archetype(name, description, traits, shadow_aspects, examples)` - Custom archetype

### Narrative Patterns
- `list_patterns()` - Available patterns
- `get_pattern_details(pattern_name)` - Pattern information
- `analyze_narrative(scenes, pattern_name, project_id, adherence_level)` - Analyze structure
- `create_custom_pattern(name, description, stages, psychological_functions, examples, based_on)` - Custom pattern

### Plotlines
- `list_plotlines()` - Available plotlines
- `get_plotline_details(plotline_name)` - Plotline information
- `develop_plotline(title, plotline, pattern, characters, project_id)` - Develop plotline
- `analyze_plotline(plot_points, plotline, project_id)` - Analyze alignment
- `create_custom_plotline(name, description, elements, examples)` - Custom plotline

### Story Generation
- `generate_outline(title, pattern, main_character, project_id, additional_characters)` - Generate outline
- `generate_scene(scene_title, pattern_stage, characters, project_id, setting, conflict)` - Generate scene
- `compile_narrative(project_id, format, include_metadata)` - Compile story
- `write_project_story(project_id, format, include_character_details, prose_style)` - Full story generation

### Knowledge Graph
- `search_nodes(query)` - Search narrative elements
- `open_nodes(names)` - Retrieve specific elements
- `read_graph()` - Access full knowledge graph

### Symbolic & Thematic
- `create_symbol(name, meaning, associations, project_id, examples)` - Create symbol
- `connect_symbols(symbol1, symbol2, relationship, project_id)` - Connect symbols

## Troubleshooting

**Import errors?**
- Ensure all dependencies are installed: `pip install -r requirements.txt`
- Check Python version: 3.10 or higher required

**Knowledge graph not working?**
- Neo4j integration is optional; system falls back to file-based storage
- Check output/knowledge_graph/ directory permissions

**Project not found?**
- Verify project ID matches: `list_writing_projects()`
- Check output/projects/ directory structure

## Contributing

Contributions are welcome! See [BEST_PRACTICES.md](./BEST_PRACTICES.md) for standards before submitting.

## Why Choose AI Writers Workshop?

1. ✅ **Theoretically Grounded** - Proven narrative frameworks
2. ✅ **Production Ready** - Battle-tested components
3. ✅ **Flexible** - Strict or creative interpretation
4. ✅ **Intelligent** - Semantic understanding of narratives
5. ✅ **Extensible** - Create custom frameworks
6. ✅ **Authoritative** - Sets industry standards
7. ✅ **Comprehensive** - Full creative writing toolset

## Resources

- **[BEST_PRACTICES.md](./BEST_PRACTICES.md)** - MCP standards and implementation guide
- **Theory References**:
  - Campbell, J. (1949). *The Hero with a Thousand Faces*
  - Vogler, C. (1992). *The Writer's Journey*
  - McKee, R. (1997). *Story: Structure, Substance, Style*
  - Jung, C.G. (1959). *The Structure and Dynamics of the Psyche*

## License

[MIT License](LICENSE)

---

**AI Writers Workshop: Where narrative science meets creative expression.**

*The definitive authority on creative writing MCPs.*
