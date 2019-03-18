# Pytroll coding guidelines and best practices

> “It is not the strongest of the species that survives,
> nor the most intelligent that survives.
> It is the one that is most adaptable to change.”
—Charles Darwin

> “It seems that perfection is attained,
> not when there is nothing more to add,
> but when there is nothing more to take away.”
—Antoine de Saint Exupéry

## Coding Style

- Language is US English.
- We generally follow the pep-8 and pep-257
- Indentation is 4 spaces (no tabs!)
- Max line length is set to 120 characters
- Every unit of code must be properly tested and documented.
- Global constants are written in capital letters, eg. PLANK_CONSTANT if they are not modified in the module and should
  be placed at the top of the module.
- About docstrings, we follow the
  [google style](https://google.github.io/styleguide/pyguide.html?showone=Comments#Comments)
- Python 2 support until end of 2019
- When in doubt, read pep 20, the Zen of Python (see appendix A)

## Maintainability Guidelines

- Functions/methods should limit lines of code (including blank lines and comments). We recommend 15 if possible.
- There should be a maximum of 3 branches in each function/method. Separate and refactor functionality to other
  functions/methods.
- Functions/methods should limit number of parameters (~5 parameters). Think of bundling arguments in helper classes
  for example.

## Style Checking

In your IDE/editor, it is highly recommended to activate/install a plugin for/script a save hook for doing automatic
style checks and/or corrections, eg autopep8, pylint, pyflakes. Most repositories will use the "stickler" github bot to
automatically check pull requests for PEP8 with the `flake8` tool.

## Working with Github

Before submitting your changes, make sure your code follow the coding style above, and that your changes are properly
covered by tests and documented. Make sure you run a style checker (eg pylint) on your code.

If you want to help develop a Pytroll package, the preferred way to contribute is to fork the original repository and
submit a pull request with your proposed changes.

The workflow in a nutshell is to:
- Fork the repository in github
- Implement the fix (with a test), it can be multiple commits
- Submit a pull request (PR) to the original upstream repository. Describe your changes and why they were needed.
  Make sure to link to any related issues or pull requests by using `#179` syntax to reference the number.
- If you need to make further changes after the PR is issued, push your new commits to your fork's branch: they will
  automatically be appended to the PR.

Pull requests should avoid committing or adding unused files (ex. .pyc files). Even if they are deleted in future
commits they should be purged from the commit history. See
[this github article](https://help.github.com/articles/removing-sensitive-data-from-a-repository/) for instructions.

- How to [create a Pull Request](https://help.github.com/articles/creating-a-pull-request/)
- How to [fork a repository](https://help.github.com/articles/fork-a-repo/)

Alternatively, patches formatted with the git format-patch command can be sent to the bdfl of the package.

The submitted work will be reviewed by the main contributors of the package, possibly engaging in a discussion on
the patch, and maybe requesting changes. Be prepared to follow up on your work.

Commit messages:
- Separate subject from body with a blank line (see "How to" link below)
- Limit the subject line to 50 characters
- Capitalize the subject line
- Do not end the subject line with a period
- Use the imperative mood in the subject line
- Wrap the body at 72 characters
- Use the body to explain what and why (not how)
- [How to Write a Git Commit Message](http://chris.beams.io/posts/git-commit/)
- [On commit messages](http://who-t.blogspot.de/2009/12/on-commit-messages.html)

## Making releases

“Release early, release often”

Versioning: [SemVer](http://semver.org/)

The procedure for releasing should be provided in each repository in a `RELEASING.md`
or similarly named file.

## Appendix A

PEP 20: The Zen of Python

- Beautiful is better than ugly.
- Explicit is better than implicit.
- Simple is better than complex.
- Complex is better than complicated.
- Flat is better than nested.
- Sparse is better than dense.
- Readability counts.
- Special cases aren’t special enough to break the rules.
- Although practicality beats purity.
- Errors should never pass silently.
- Unless explicitly silenced.
- In the face of ambiguity, refuse the temptation to guess.
- There should be one– and preferably only one –obvious way to do it.
- Although that way may not be obvious at first unless you’re Dutch.
- Now is better than never.
- Although never is often better than right now.
- If the implementation is hard to explain, it’s a bad idea.
- If the implementation is easy to explain, it may be a good idea.
- Namespaces are one honking great idea – let’s do more of those!
