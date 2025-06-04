- 👋 Hi, I’m @Layakboy
- 👀 I’m interested in Travelling
- 🌱 I’m currently learning Code
- 💞️ I’m looking to collaborate on Trusted Team
- 📫 How to reach me no one can reach me
- 😄 Pronouns: ...
- ⚡ Fun fact: im gold

<!---
Layakboy/Layakboy is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

## Talos Scraping Notes

The `ioc_analyzer.py` script queries [Talos Intelligence](https://talosintelligence.com) to enrich IOCs. Talos may block requests that do not look like they originate from a browser. If lookups fail you can supply additional headers or cookies using a JSON configuration file. Pass the path to this file when prompted in the UI.

Example `talos_config.json`:

```json
{
  "headers": {
    "Referer": "https://talosintelligence.com/",
    "Accept-Language": "en-US,en;q=0.9"
  },
  "cookies": {
    "your_cookie": "value"
  }
}
```

Without appropriate headers or cookies Talos lookups may fail or return unexpected results.
