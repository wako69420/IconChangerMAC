# Contributing to Icon Changer

First off, thank you for considering contributing to Icon Changer! 
**Note:** As stated in the README, this project is currently **archived** and was primarily a learning project. Active development and maintenance have ceased.

However, if you wish to fork this repository or if development resumes in the future, please follow these guidelines.

## Pull Requests

1. **Fork the Repository:** Create your own fork and branch off `main`.
2. **Code Quality:** Ensure your code is clean, readable, and follows standard Swift conventions.
3. **Testing:** Test your changes locally. Icon Changer interacts with native macOS APIs (like `NSWorkspace`), so ensure your changes do not cause unintended side effects (e.g., crashing Finder, sandbox violations).
4. **Descriptive PRs:** Provide a clear and detailed explanation of what your Pull Request does, why it's necessary, and any trade-offs you made.
5. **No Malicious Code:** Any code that attempts to bypass macOS security maliciously or harms the user's system will be immediately rejected.

## Issues

Since the project is archived, we may not actively monitor or respond to new issues. If you do open an issue, please ensure:
- You have searched existing issues to avoid duplicates.
- You provide a clear description of the bug or feature request.
- You include steps to reproduce (for bugs).
- You specify your macOS version.

## Code Quality

- Avoid adding hacky shell scripts (`osascript`, `killall`) unless absolutely necessary. We prefer using native Apple APIs (`NSWorkspace`, `FileManager`) whenever possible.
- Keep the UI native-feeling using standard SwiftUI components.
