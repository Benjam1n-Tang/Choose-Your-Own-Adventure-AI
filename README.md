# Choose Your Own Adventure AI

An interactive, AI-powered choose your own adventure game that creates dynamic, personalized narratives using artificial intelligence to generate unique storytelling experiences.

## 🎮 Description

This project combines the classic choose-your-own-adventure format with modern AI technology to create unlimited, procedurally generated stories. Players make choices that influence the narrative direction, while AI generates contextually appropriate story content, ensuring no two playthroughs are exactly the same.

## ✨ Features

- **AI-Generated Narratives**: Dynamic story creation using advanced language models
- **Interactive Decision Making**: Multiple choice options that impact story progression
- **Persistent Game State**: Save and resume adventures across sessions
- **Character Development**: Track player choices and character progression
- **Multiple Genres**: Support for various story themes (fantasy, sci-fi, mystery, etc.)
- **Customizable Settings**: Adjust story length, complexity, and content preferences
- **Rich Text Interface**: Engaging user interface for immersive storytelling

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- OpenAI API key (or other supported AI service)
- Required Python packages (see `requirements.txt`)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Benjam1n-Tang/Choose-Your-Own-Adventure-AI.git
cd Choose-Your-Own-Adventure-AI
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up your API keys:
```bash
# Create a .env file in the root directory
cp .env.example .env
# Edit .env and add your API keys
```

4. Run the application:
```bash
python main.py
```

## 🔧 Configuration

Create a `.env` file in the root directory with the following variables:

```env
OPENAI_API_KEY=your_openai_api_key_here
MAX_STORY_LENGTH=1000
DEFAULT_GENRE=fantasy
SAVE_GAMES_DIR=./saves
DEBUG=False
```

## 📖 Usage

1. **Start a New Adventure**: Launch the application and choose "New Game"
2. **Select Genre**: Pick from available story themes
3. **Create Character**: Set up your character's background and traits
4. **Make Choices**: Read the narrative and select from AI-generated options
5. **Save Progress**: Use the save feature to continue later
6. **Load Game**: Resume previous adventures from the main menu

### Example Gameplay Flow

```
> You find yourself at the entrance of a mysterious cave...
> What do you choose to do?

A) Enter the cave cautiously
B) Look for another path around
C) Call out to see if anyone responds
D) Light a torch before proceeding

> Choice: A

> As you step into the cave, the air grows cold and damp...
```

## 🏗️ Project Structure

```
Choose-Your-Own-Adventure-AI/
├── main.py                 # Main application entry point
├── game/
│   ├── __init__.py
│   ├── adventure.py        # Core game logic
│   ├── ai_generator.py     # AI story generation
│   ├── character.py        # Character management
│   └── save_system.py      # Game state persistence
├── ui/
│   ├── __init__.py
│   ├── interface.py        # User interface components
│   └── display.py          # Text formatting and display
├── config/
│   ├── __init__.py
│   └── settings.py         # Configuration management
├── saves/                  # Saved game files
├── templates/              # Story templates and prompts
├── requirements.txt        # Python dependencies
├── .env.example           # Environment variables template
└── README.md              # This file
```

## 🔌 API Integration

This project supports multiple AI providers:

- **OpenAI GPT Models**: Primary integration for story generation
- **Anthropic Claude**: Alternative AI provider support
- **Local Models**: Support for self-hosted language models

## 🎯 Customization

### Adding New Genres

Create new story templates in the `templates/` directory:

```python
# templates/horror.py
HORROR_PROMPT = """
Generate a horror-themed choose your own adventure segment...
"""
```

### Modifying AI Behavior

Adjust the AI generation parameters in `config/settings.py`:

```python
AI_SETTINGS = {
    "temperature": 0.8,
    "max_tokens": 300,
    "presence_penalty": 0.1,
    "frequency_penalty": 0.1
}
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### Development Setup

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Add tests for new functionality
5. Commit your changes (`git commit -m 'Add amazing feature'`)
6. Push to the branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

### Code Style

- Follow PEP 8 guidelines
- Use meaningful variable and function names
- Add docstrings for functions and classes
- Include type hints where appropriate

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- OpenAI for providing the GPT API
- The choose-your-own-adventure book series for inspiration
- Contributors and beta testers

## 📧 Contact

Benjamin Tang - [@Benjam1n-Tang](https://github.com/Benjam1n-Tang)

Project Link: [https://github.com/Benjam1n-Tang/Choose-Your-Own-Adventure-AI](https://github.com/Benjam1n-Tang/Choose-Your-Own-Adventure-AI)

## 🔮 Future Enhancements

- [ ] Multiplayer support for collaborative storytelling
- [ ] Image generation for story scenes
- [ ] Voice narration capabilities
- [ ] Mobile app version
- [ ] Story sharing and community features
- [ ] Advanced character stat systems
- [ ] Integration with more AI providers

---

**Enjoy your AI-powered adventures!** 🚀✨
