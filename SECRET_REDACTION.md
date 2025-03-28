# Secret Redaction in Warp

## Overview
Secret Redaction is a feature in Warp that automatically redacts secrets and sensitive information in your terminal output, including passwords, IP addresses, API keys, and personally identifiable information (PII). This feature enhances security by preventing sensitive data from being exposed in terminal logs.

## How to Access Secret Redaction
- Secret Redaction is disabled by default. To enable it:
  - Open **Settings > Privacy > Secret Redaction**.
  - Alternatively, type "Secret Redaction" in the Command Palette to toggle it.

## How It Works
- Secret Redaction attempts to detect sensitive data using a list of default regex patterns and masks it with asterisks.
- Clicking on a redacted secret will display a tooltip that allows you to reveal the secret or copy its contents.
- When copying terminal output containing secrets, it will be copied as asterisks (e.g., `echo password` becomes `echo ********`) unless revealed or copied from the tooltip.
- Note that secret redaction is not applied in shared sessions.

### Custom Regex Patterns
- You can add additional custom regex patterns for secrets you want to include by navigating to **Settings > Privacy > Secret Redaction > Custom Secret Redaction**.

### AI Interactions
- Secret redaction always applies to AI interactions, regardless of this setting. Your secrets will never be sent to AI.

## Default Regex Patterns
Here is a list of the default regular expressions that Warp uses to identify secrets:

| Secret Type                               | Regex Pattern                                                                                     |
|-------------------------------------------|--------------------------------------------------------------------------------------------------|
| IP V4 Address                             | \b((25[0-5]|(2[0-4]|1\d|[1-9]|)\d)\.?\b){4}\b                                                  |
| IP V6 Address                             | \b((([0-9A-Fa-f]{1,4}:){1,6}:)|(([0-9A-Fa-f]{1,4}:){7}))([0-9A-Fa-f]{1,4})\b                  |
| Slack App Token                           | \bxapp-[0-9]+-[A-Za-z0-9_]+-[0-9]+-[a-f0-9]+\b                                                |
| Phone Number                              | \b(\+\d{1,2}\s)?\(?\d{3}\)?[\s.-]\d{3}[\s.-]\d{4}\b                                           |
| AWS Access ID                             | \b(AKIA|A3T|AGPA|AIDA|AROA|AIPA|ANPA|ANVA|ASIA)[A-Z0-9]{12,}\b                                  |
| MAC Address                               | \b((([a-zA-z0-9]{2}[-:]){5}([a-zA-z0-9]{2}))|(([a-zA-z0-9]{2}:){5}([a-zA-z0-9]{2})))\b        |
| Google API Key                            | \bAIza[0-9A-Za-z-_]{35}\b                                                                        |
| Google OAuth ID                           | \b[0-9]+-[0-9A-Za-z_]{32}\.apps\.googleusercontent\.com\b                                       |
| Github Classic Personal Access Token      | \bghp_[A-Za-z0-9_]{36}\b                                                                          |
| Github Fine Grained Personal Access Token  | \bgithub_pat_[A-Za-z0-9_]{82}\b                                                                  |
| Github OAuth Access Token                  | \bgho_[A-Za-z0-9_]{36}\b                                                                          |
| Github User to Server Token                | \bghu_[A-Za-z0-9_]{36}\b                                                                          |
| Github Server to Server Token              | \bghs_[A-Za-z0-9_]{36}\b                                                                          |
| Heroku API Key                            | \b[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}\b                 |
| Stripe Key                                | \b(?:r|s)k_(test|live)_[0-9a-zA-Z]{24}\b                                                        |
| Firebase Auth Domain                       | \b([a-z0-9-]){1,30}(\.firebaseapp\.com)\b                                                       |

This guide will assist users in understanding and utilizing the Secret Redaction feature effectively within the Warp terminal.
