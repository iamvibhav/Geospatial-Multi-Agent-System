# 🤖 Hugging Face Agents: Multi-Agent Geospatial Analysis System

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A sophisticated hierarchical multi-agent system that finds Batman filming locations worldwide, calculates cargo plane transfer times, and creates interactive geospatial visualizations using cutting-edge AI technologies.

## 🚀 Project Overview

This repository contains an advanced multi-agent geospatial analysis system built with modern AI frameworks:

**🌍 Multi-Agent Geospatial Analysis System** - A hierarchical multi-agent system that finds Batman filming locations worldwide, calculates cargo plane transfer times, and creates interactive maps with color-coded travel times.

## 📋 Table of Contents

- [Features](#-features)
- [Installation](#-installation)
- [Usage](#-usage)
- [Architecture](#-architecture)
- [Technologies](#-technologies)
- [Contributing](#-contributing)
- [License](#-license)

## ✨ Features

### 🌍 Multi-Agent Geospatial Analysis System

- **Hierarchical Multi-Agent Architecture**: Manager agent orchestrates specialized web agents
- **Global Location Discovery**: Automatically finds Batman filming locations worldwide
- **Cargo Plane Transfer Calculations**: Precise travel time calculations using great-circle distance
- **Interactive Mapping**: Beautiful scatter plots with color-coded travel times
- **Supercar Factory Integration**: Matches filming locations with supercar factories
- **Quality Assurance**: Automated reasoning validation and plot verification
- **Real-time Web Research**: Dynamic information gathering from multiple sources
- **Geospatial Visualization**: Interactive world maps with Plotly integration

## 🛠️ Installation

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- API keys for various services (see Configuration section)

### Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd hugging-face-agents
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Install Jupyter extensions** (optional)
   ```bash
   pip install jupyter_contrib_nbextensions
   jupyter contrib nbextension install --user
   ```

### Configuration

Set up your API keys as environment variables:

```bash
# Required for Multi-Agent System
export SERPAPI_API_KEY="your_serpapi_key"
export OPENAI_API_KEY="your_openai_key"
export TOGETHER_API_KEY="your_together_api_key"
```

## 🚀 Usage

### Multi-Agent Geospatial Analysis

1. **Open the notebook**
   ```bash
   jupyter notebook Smolagents_Multiagent.ipynb
   ```

2. **Run the cells sequentially** to:
   - Install dependencies (`smolagents[litellm]`, `plotly`, `geopandas`, `shapely`, `kaleido`)
   - Set up the cargo travel time calculator with great-circle distance calculations
   - Initialize the multi-agent system with manager and web agents
   - Execute the geospatial analysis to find Batman filming locations
   - Generate interactive maps with color-coded travel times
   - Validate results with automated quality checks

3. **Expected Output**: Interactive world map showing Batman filming locations and supercar factories with color-coded travel times from Gotham (40.7128° N, 74.0060° W)

## 🏗️ Architecture

### Multi-Agent System Architecture

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Manager Agent │───▶│   Web Agent     │───▶│  Travel Time    │
│   (Orchestrator)│    │   (Researcher)  │    │  Calculator     │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         │                       │                       │
         ▼                       ▼                       ▼
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│  Quality Check  │    │  Location Data  │    │  Geospatial    │
│  & Validation   │    │  Collection     │    │  Visualization  │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

### Agent Hierarchy

- **Manager Agent**: Orchestrates the entire workflow, manages planning intervals, and validates final outputs
- **Web Agent**: Specialized in web research, location discovery, and information gathering
- **Travel Time Calculator**: Custom tool for precise cargo plane transfer time calculations
- **Quality Assurance**: Automated validation of reasoning and visualization outputs

## 🛠️ Technologies

### Core Frameworks
- **Smolagents**: Multi-agent orchestration and tool integration
- **Hugging Face Hub**: Model hosting and inference
- **Together AI**: High-performance model inference

### AI Models
- **Qwen/Qwen2.5-Coder-32B-Instruct**: Primary coding and reasoning model
- **DeepSeek-R1**: Manager agent for complex planning and orchestration
- **GPT-4o**: Multimodal reasoning and validation

### Data Processing & Visualization
- **Pandas**: Data manipulation and analysis
- **Plotly**: Interactive geospatial visualizations
- **GeoPandas**: Geographic data processing
- **Shapely**: Geometric operations
- **Kaleido**: Static image export for Plotly

### Web & Search
- **Google Search API**: Web search capabilities
- **Serper API**: Alternative search provider
- **Web scraping tools**: Information extraction

### Development & Utilities
- **Jupyter**: Interactive development environment
- **Pillow**: Image processing and manipulation
- **Math**: Mathematical calculations for great-circle distance

## 📊 Key Features in Detail

### Cargo Plane Transfer Calculator

The system includes a sophisticated travel time calculator that:
- Uses great-circle distance calculations for accurate global measurements
- Accounts for non-direct routes (10% buffer for air traffic and routing)
- Includes takeoff and landing procedures (1 hour buffer)
- Supports configurable cruising speeds (default: 750 km/h)
- Provides precise time estimates in hours with 2 decimal precision
- Handles Earth's curvature for long-distance calculations

### Quality Assurance System

Automated validation ensures:
- Correct plotting methods (px.scatter_map for optimal visualization)
- Data integrity and completeness (minimum 6 data points)
- Logical consistency in reasoning and calculations
- Visual output quality and proper color coding
- Geospatial accuracy and coordinate validation

### Multi-Agent Coordination

The hierarchical system features:
- **Planning Intervals**: Manager agent reviews progress every 4-5 steps
- **Tool Integration**: Seamless integration of custom tools with web search
- **State Management**: Persistent state tracking across agent interactions
- **Error Handling**: Robust error recovery and validation
- **Scalable Architecture**: Easy addition of new specialized agents

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/amazing-feature`)
3. **Commit your changes** (`git commit -m 'Add amazing feature'`)
4. **Push to the branch** (`git push origin feature/amazing-feature`)
5. **Open a Pull Request**

### Development Guidelines

- Follow PEP 8 style guidelines
- Add comprehensive docstrings
- Include unit tests for new features
- Update documentation as needed
- Ensure all notebooks run without errors
- Test with different geographic locations and scenarios

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Hugging Face** for the excellent agents course and frameworks
- **Smolagents** team for the powerful multi-agent orchestration system
- **Together AI** for hosting the open-source models
- **OpenAI** for providing the GPT models for validation

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/your-repo/issues) page
2. Create a new issue with detailed information
3. Join our [Discussions](https://github.com/your-repo/discussions) for community support

---

**Made with ❤️ by the AI Agents Community**

*This project is part of the [Hugging Face Agents Course](https://www.hf.co/learn/agents-course), a comprehensive guide from beginner to expert in building AI agents.* 