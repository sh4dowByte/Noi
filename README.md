
# Noi Mode  
**Fast Access to the World of AI and Development in One Place!**  

*Organize your favorite AI and development tools, ready to use anytime.*

---

## What is Noi Mode?  
Noi Mode is a JSON-based configuration project that helps you organize and quickly access AI and development tools. From ChatGPT to GitHub, everything is neatly structured, customizable, and automatically synced. Paired with the Noi app, it’s perfect for developers, AI enthusiasts, or anyone aiming for maximum productivity!

- **Current Version**: 0.1.11  
- **Sync**: [configs/noi.json](https://raw.githubusercontent.com/sh4dowByte/Noi/refs/heads/main/configs/noi.json)  
- **Noi App**: Visit [https://noi.nofwl.com/](https://noi.nofwl.com/) for more info or to download the app.

---

## Key Features  
- **Hierarchical Categories**: Separate AI and Dev tools with a flexible tree structure.  
- **Instant Access**: Each tool comes with a direct URL to your favorite services.  
- **Easy Sync**: Update the tool list from a public URL anytime.  
- **Noi App Integration**: Pair it with the desktop app for a seamless experience.  

---

## About the Noi App  
The Noi app is a cross-platform desktop application (available for Mac, Windows, and Linux) designed to speed up access to AI and development tools. According to [https://noi.nofwl.com/](https://noi.nofwl.com/), Noi aims to "Power Your World with AI - Explore, Extend, Empower". It leverages the `noi.json` configuration to provide an organized, efficient interface.

- **Download**: Check [https://noi.nofwl.com/](https://noi.nofwl.com/) for download links or installation instructions.  
- **macOS Note**: If you see *"Noi is damaged and can’t be opened"*, run this command in Terminal:  
  ```bash
  xattr -cr /Applications/Noi.app
  ```

---

## Configuration Structure  
Noi Mode uses a JSON file to manage everything. Here’s a quick example:  

```json
{
  "name": "Noi Mode",
  "version": "0.1.11",
  "sync": "https://raw.githubusercontent.com/sh4dowByte/Noi/refs/heads/main/configs/noi.json",
  "modes": [
    {
      "id": "noi@ai",
      "parent": 0,
      "dir": true,
      "text": "AI"
    },
    {
      "id": "noi:chatgpt",
      "parent": "noi@ai",
      "text": "ChatGPT",
      "url": "https://chatgpt.com"
    }
  ]
}
```

### Field Breakdown  
- **`id`**: Unique identifier for categories or tools (e.g., `noi@ai` for a category, `noi:chatgpt` for a tool).  
- **`parent`**: Parent ID (0 for root, or another category’s ID).  
- **`dir`**: `true` for categories, omitted for tools.  
- **`text`**: Display name.  
- **`url`**: Direct link to the tool (optional).  

---

## Tool List  
### AI  
- **[ChatGPT](https://chatgpt.com)** - Conversational AI from OpenAI.  
- **[Deepseek](https://chat.deepseek.com)** - Smart conversational AI.  
- **[Grok AI](https://grok.com/?referrer=website)** - Exploration AI from xAI.  
- **[Claude](https://claude.ai)** - Conversational AI from Anthropic.  
- **[Midjourney](https://www.midjourney.com)** - AI art generator.  
*(and 16 more AI tools!)*  

### Dev  
- **[GitHub](https://github.com)** - Code collaboration platform.  
*(Plenty of room to expand this category!)*  

---

## How to Use  
1. **Grab the Config**: Download `noi.json` from [here](https://raw.githubusercontent.com/sh4dowByte/Noi/refs/heads/main/configs/noi.json).  
2. **Install the Noi App**: Visit [https://noi.nofwl.com/](https://noi.nofwl.com/) to get the app.  
3. **Customize**: Add or edit your favorite tools in the JSON.  
4. **Sync**: Let the Noi app pull updates from the sync URL.  

---

## Contributing  
We want Noi Mode and the Noi app to grow with your help!  
- **Add Tools**: Suggest new AI or Dev tools via a pull request!  
- **Fix Bugs**: Spot an issue in the JSON or app? Report it in Issues.  
- **Share Ideas**: Propose new features or enhancements.  

1. Fork this repository.  
2. Edit `configs/noi.json`.  
3. Commit and submit a pull request.  

---

## Usage Example  
Imagine opening the Noi app and seeing:  
- **AI**  
  - ChatGPT → Click, straight to [chatgpt.com](https://chatgpt.com).  
  - Grok AI → Click, explore [grok.com](https://grok.com/?referrer=website).  
- **Dev**  
  - GitHub → Click, start coding at [github.com](https://github.com).  

---

This translation maintains the original structure and excitement while ensuring natural English for a global GitHub audience. Let me know if you’d like any tweaks!
