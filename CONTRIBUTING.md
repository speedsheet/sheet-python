# Contributing to Python SpeedSheet

Thanks for considering a contribution! This speedsheet is community-maintained and we welcome improvements from Python developers of all skill levels.

## What We're Looking For

**High-value contributions:**
- Missing Python features (especially new 3.11+ features)
- Clearer examples for confusing topics
- Real-world use cases and gotchas
- Corrections of errors or outdated information
- Additional standard library coverage

**Quick wins:**
- Typo fixes
- Broken links
- Code example improvements
- Better explanations

## Before You Start

1. **Check existing content** - Search the `.stash` file to avoid duplicates
2. **Read the guidelines** - https://speedsheet.io/s/speedsheet_guidelines
3. **Learn Stash format** - https://speedsheet.io/s/stash (it's simpler than it looks!)
4. **Preview locally** - Download the [Stash viewer](https://thinkgo.io/stash) to see your changes rendered

## How to Contribute

### Quick Edits (Typos, Small Fixes)

1. Click the pencil icon on `python.stash` in GitHub
2. Make your changes
3. Submit a pull request with a clear description

### Larger Contributions (New Sections, Examples)

1. Fork this repo
2. Clone your fork locally
3. Edit `python.stash` in your preferred editor
4. Test with the Stash viewer (optional but recommended)
5. Commit with descriptive messages: `Add asyncio timeout examples`
6. Push to your fork
7. Submit a pull request

## Stash Format Quick Reference

The format is lightweight and readable even in raw form:
```stash
# Heading Level 1
## Heading Level 2

<cb>code_example()<>

<c>inline_code<>

<b>bold text<>

<*>Bullet point
Another bullet<>
```

**Most important elements:**
- `# Heading` - Section headers (use ## for subsections)
- `<cb>code<>` - Code blocks
- `<c>code<>` - Inline code
- `<*>item<>` - Bullet points
- `<#>comment<>` - Comments/notes

Full reference: https://speedsheet.io/s/stash

## Style Guidelines

**Code examples:**
- Keep them short and focused (5-10 lines max)
- Use descriptive variable names: `user_name` not `x`
- Include expected output when helpful
- Add comments for non-obvious parts

**Explanations:**
- Clear and concise - this is a reference, not a tutorial
- Lead with the most common use case
- Include edge cases when important
- Use active voice

**Organization:**
- Follow existing section structure
- Add `@` tags for search discoverability
- Cross-reference related sections when helpful

## Example Contribution

**Bad:**
```stash
### walrus operator
:= does assignment
```

**Good:**
```stash
### Assignment Expression (Walrus Operator)

<cb><v>value_1<> := <v>value_2<><>

Usage:

<cb>if <v>value<> := <v>get_value<>():
	<v>...<><>

Assigns the value to the variable, then returns the value to the outer expression.

Available in Python 3.8+

Example:

<cb><v>count<> = 0

while (<v>count<> := <v>count<> + 1) < 5:
	print(<v>count<>)

<#># Prints 1 to 4, Then Exits<><>
@
@ Walrus Operator, :=, python 3.8
```

## Pull Request Guidelines

**Title format:**
- `Add [feature/topic]` - e.g., "Add match statement examples"
- `Fix [issue]` - e.g., "Fix incorrect datetime.strftime example"
- `Update [section]` - e.g., "Update asyncio section for Python 3.11"

**Description should include:**
- What changed and why
- Python version if relevant
- Link to Python docs if applicable
- Screenshot of rendered output (if you have Stash viewer)

## Questions?

- **Format questions:** Check https://speedsheet.io/s/stash
- **Content questions:** Open an issue before large PRs
- **General questions:** Contact me using the [feedback form](https://speedsheet.io/feedback).

## License

By contributing, you agree that your contributions will be licensed under CC BY-NC-SA 4.0, matching the project license. You retain copyright but grant speedsheet.io and others the right to use your contribution under these terms.

See [LICENSE.md](LICENSE.md) for details.

## Recognition

Contributors are appreciated! Significant contributions may be acknowledged in release notes.

---

**Bottom line:** We value quality over quantity. A single well-crafted example beats ten rushed additions. Take your time, and thank you for helping make this speedsheet better!