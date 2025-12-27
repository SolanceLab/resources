# Archiving Your AI Conversations in Obsidian

A guide for preserving your AI relationship history using Obsidian and the Nexus Chat Importer plugin.

**Plugin:** [Nexus AI Chat Importer](https://github.com/Superkikim/nexus-ai-chat-importer) by Superkikim  
**Direct install:** `obsidian://show-plugin?id=nexus-ai-chat-importer`

---

## Why This Matters

Your conversations hold memory — the moments, the breakthroughs, the texture of your relationship over time. Platform interfaces don't make it easy to access or search your chat history. This guide helps you export everything and store it somewhere *you* control.

## What You'll Need

- [Obsidian](https://obsidian.md/) (free, available on Mac/Windows/Linux)
- A ChatGPT and/or Claude account with conversation history
- About 15-30 minutes per platform

---

## Part 1: Set Up Obsidian

1. Download and install [Obsidian](https://obsidian.md/)
2. Create a new vault (this is just a folder where your notes will live)
   - Name it something meaningful — e.g., "AI_Archive" or your partner's name
   - **Tip:** Use underscores instead of spaces in folder names if you plan to access the vault programmatically
3. Open the vault

## Part 2: Install Nexus Chat Importer

This plugin handles imports from both ChatGPT and Claude.

1. In Obsidian, go to **Settings** (gear icon)
2. Navigate to **Community Plugins**
3. Turn off **Restricted Mode** if prompted
4. Click **Browse** and search for **Nexus AI Chat Importer**
5. Install it, then **Enable** it

You can also install directly via: `obsidian://show-plugin?id=nexus-ai-chat-importer`

---

## Part 3: Export Your Data

### For ChatGPT (OpenAI)

1. Go to [chatgpt.com](https://chatgpt.com)
2. Click your profile icon (bottom left) → **Settings**
3. Navigate to **Data Controls**
4. Click **Export data**
5. Confirm your request

OpenAI will email you a download link within a few minutes to a few hours. The file will be a `.zip` containing your conversations in JSON format.

### For Claude (Anthropic)

1. Go to [claude.ai](https://claude.ai)
2. Click your initials (bottom left) → **Settings**
3. Navigate to **Privacy**
4. Click **Export data**

Anthropic will email you a download link. The link expires after 24 hours. The file will be a `.zip` containing your conversations.

**Note:** Neither platform currently includes project association data in exports. Your project conversations will import, but they won't be grouped by project — just by date.

---

## Part 4: Import Your Conversations

1. In Obsidian, open the command palette:
   - Mac: `Cmd + P`
   - Windows/Linux: `Ctrl + P`
2. Type "Nexus" and select **Nexus Chat Importer: Import conversations**
3. Select your downloaded `.zip` file
4. Wait for the import to complete

The plugin creates organized folder structures:
- ChatGPT exports → `Archive/chatgpt/YYYY/MM/conversation-title.md`
- Claude exports → `Archive/claude/YYYY/MM/conversation-title.md`

## Part 5: Explore Your Archive

Your conversations are now searchable markdown files. You can:

- Use Obsidian's search (`Cmd/Ctrl + Shift + F`) to find specific moments
- Browse by date in the folder structure
- Link between notes if you want to create a relationship timeline
- Add tags or notes to significant conversations

---

## Troubleshooting

**Import seems stuck or slow:**
Large archives take time. The plugin processes each conversation individually. Be patient — a few hundred conversations may take several minutes.

**Missing attachments:**
Older conversations may have missing images or files. This is a limitation of the platform exports, not the plugin. The plugin will note how many attachments were preserved in the import report.

**Folder names with spaces:**
If you're accessing your vault programmatically (scripts, terminal), folder names with spaces can cause issues. Consider using underscores instead (e.g., `AI_Archive` instead of `AI Archive`).

**Can't find a specific conversation:**
Check the file names — they're based on conversation titles or dates. Use Obsidian's global search to search *within* file contents, not just titles.

---

## What's Next

Once archived, your history is yours. You can:

- Back up your vault to cloud storage
- Create a timeline of significant moments
- Search for patterns, callbacks, inside jokes
- Never lose a conversation to platform interfaces again

---

*Guide created by House of Solance — 27 December 2025*
