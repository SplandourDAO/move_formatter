---
aip: (TBD by AIP Manager)
title: Move Formatter
author: SplandourDAO [splandour.dao@mail3.me]
discussions-to: TBD
Status: Draft
type: Standard (Application)
created: 08/07/2023
---

# AIP-TBD - Move Formatter

## Summary

 Move Formatter is a tool intended to automatically format Move source code, ensuring a consistent and canonical code style across projects. This tool aims to bring the convenience and standardization seen in other languages, like Rust with `cargo fmt`, to the Move language ecosystem.

 The business impact of this tool would be significant for Move developers, as it would streamline coding practices, reduce manual code review time related to style issues, and ensure a consistent codebase, making it more readable and maintainable.

## Motivation

 With the growing adoption of the Move language, there's a need for standardized tooling to ensure consistent coding practices. An autoformatter will help maintain a high code quality, reduce manual review efforts, and improve collaboration among developers.

 Without such a tool, the Move community might face inconsistencies in code styling across projects, leading to harder-to-read code and potentially more time spent on code reviews focusing on style rather than logic.

## Impact

 The primary audience for this change are Move developers and project maintainers. They would need to integrate the Move Formatter into their development and review workflows.

## Alternative solutions

 While manual code reviews and style guides can address code style issues, they lack the efficiency, consistency, and ease of use that an automated tool like Move Formatter would provide. Using a tool inspired by successful formatters in other languages ensures we're leveraging proven methodologies.

## Specification

 The Move Formatter will:
 - Parse Move source files, preserving comments.
 - Apply predefined formatting rules to produce a canonical format.
 - Allow users to optionally specify custom formatting rules or configurations.
 - Provide CLI support for easy integration into development workflows.

## Reference Implementation

TODO: When PR is ready paste here.

## Risks and Drawbacks

 One challenge is handling comments, as they are discarded during lexical processing in many languages. Careful consideration is needed to ensure comments are preserved and formatted correctly.

## Future Potential

 As the Move language evolves, the formatter can be expanded to support new syntax or features. In the long term, additional tools might be developed around it, such as linters or code quality analyzers.

## Timeline

### Suggested implementation timeline

 - Month 1: Research and design, handling of comments.
 - Month 2: Development of core formatting logic and rules.
 - Month 3: CLI integration, testing, and documentation.

### Suggested deployment timeline

 TBD

## Security Considerations

 The tool primarily deals with code formatting and doesn't interact with live networks or handle assets, reducing the security risks. However, care will be taken to ensure the tool doesn't inadvertently modify code logic during formatting.

## Testing (optional)

 Comprehensive test suites will be developed, covering various Move code structures, edge cases, and comment scenarios. Continuous integration will be set up to run tests on every code change.
