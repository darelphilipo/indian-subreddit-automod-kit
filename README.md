# 🇮🇳 Indian AutoModerator Rules Kit (Copy-Paste Ready)

A curated set of **copy-paste AutoModerator rules** designed specifically for Indian subreddits.

This repo targets the most common moderation pain points in Indian communities:

- Spam & low-karma accounts
- Donation / crowdfunding scams
- Phone number leaks (doxxing)
- Hindi abuses / slur filtering
- Caste / communal bait keywords
- Clickbait titles
- "Members Only" / "Verified Voice" threads

---

# 🚀 Quick Start

### Step 1: Open your AutoModerator config
Go to:

**Subreddit → Mod Tools → AutoModerator → Edit Config**

### Step 2: Copy-paste rules
Copy rules from the `/automod/` folder into your config.

### Step 3: Save

---

# 📌 Copy-Paste Rules (Ready YAML)

| Rule | File |
|------|------|
| Members Only / Verified Voice Mode | `automod/members_only_mode.yaml` |
| Low karma submission filter | `automod/low_karma_submission_filter.yaml` |
| Minimum account age | `automod/account_age_limit.yaml` |
| Filter posts with multiple reports | `automod/multiple_reports_filter.yaml` |
| Shadowban specific users | `automod/shadowban_users.yaml` |
| Filter moderation meta discussions | `automod/moderation_keywords_filter.yaml` |
| Crowdfunding / donation scam domains | `automod/crowdfunding_filter.yaml` |
| Hindi abuses regex filter | `automod/hindi_abuses_filter.yaml` |
| Clickbait detector | `automod/clickbait_detector.yaml` |
| Remove link-only self posts | `automod/link_only_selfpost.yaml` |
| Caste/religion keyword filter | `automod/caste_religion_filter.yaml` |
| Phone number / doxxing detection | `automod/phone_number_filter.yaml` |

---

# 🧨 Abuse / Hate / Keyword Lists (Community Editable)

The keyword lists are separated into the `/filters/` folder so contributors can improve them without breaking YAML formatting.

| List Type | File |
|----------|------|
| Hindi abuses (plain list) | `filters/hindi_abuses_plain_list.txt` |
| Hindi abuses (regex format, copy-paste) | `filters/hindi_abuses_regex_copy_paste.txt` |
| Crowdfunding domains (plain list) | `filters/crowdfunding_domains_india.txt` |
| Caste/religion keywords (plain list) | `filters/caste_religion_keywords.txt` |
| Moderation keywords | `filters/moderation_keywords.txt` |

---

# 🤖 LLM Prompt: Convert Plain Keyword List into Copy-Paste Regex Rule

AutoModerator and Reddit Automations require regex formatting.

To regenerate a paste-ready regex rule from a plain list:

📌 Open `docs/prompts.md`

---

# 🤝 Contributing

Want to add:
- new scam domains?
- more slur variations?
- better regex patterns?
- regional language abuse lists?

See: `docs/contributing.md`

---

# ⚠️ Disclaimer

These rules are shared for community safety and moderation convenience.

Always test rules in your subreddit before enabling strict actions like `remove`.

---

# ⭐ Support

If this repo helped you, star it and share it with other Indian mods.
