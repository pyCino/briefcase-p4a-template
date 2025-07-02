# Briefcase P4A Template

**Cookiecutter template for Python-for-Android projects.** Used by the Briefcase P4A Backend.

## Purpose

Generates project structure for building Android APKs using Python-for-Android through Briefcase. Creates necessary configuration files and directory structure for P4A builds.

## Usage

Automatically used by the [Briefcase P4A Backend](https://github.com/pyCino/briefcase-p4a-backend). Direct usage not typically required.

### Automatic Usage

```bash
pip install git+https://github.com/pyCino/briefcase-p4a-backend.git
briefcase new
# Select "Android" platform and "p4a" format
briefcase build android p4a
```

### Manual Usage

```bash
pip install cookiecutter
cookiecutter https://github.com/pyCino/briefcase-p4a-template.git
```

## Template Structure

```
{{cookiecutter.formal_name}}/
├── briefcase.toml
└── pyproject.toml
```

## Template Variables

| Variable | Description | Example |
|----------|-------------|---------|
| `formal_name` | Application display name | "My App" |
| `class_name` | Python class name | "MyApp" |
| `module_name` | Python module name | "myapp" |
| `bundle_identifier` | Android package ID | "com.example.myapp" |
| `python_version` | Target Python version | "3.11" |

## Generated Files

**briefcase.toml**
Briefcase-specific configuration for P4A build process:
- Application metadata
- Build paths and settings
- P4A-specific configuration

**pyproject.toml**
Standard Python project configuration:
- Project metadata
- Dependencies
- Build system configuration

## Related Projects

- [Briefcase P4A Backend](https://github.com/pyCino/briefcase-p4a-backend)
- [Briefcase Kivy Bootstrap](https://github.com/pyCino/briefcase-kivy-bootstrap)
- [Briefcase](https://github.com/beeware/briefcase)
- [Python-for-Android](https://github.com/kivy/python-for-android)

## License

MIT License

---

**Al pyCino** 