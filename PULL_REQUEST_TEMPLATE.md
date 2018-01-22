## Description

Please describe your pull request. If it fixes a bug or resolves a feature request, be sure to link to that issue. When linking to an issue, please use Github's `#...` in the description of the pull request.

## Checklist before merging Pull Requests

- [ ] If functionality could have architectural implications or controversial, have a discussion with the team. Ideally, prior to coding to save effort. Also making sure to point to the specs process for large changes.
- [ ] Ensure any user, deployer or developer documentation is updated.
- [ ] If a change affects an external API, be sure to update docs/rest\_api.md.
- [ ] Testing:
  - [ ] Ensure tests pass after making your changes by running `py.test tests/unit tests/stress.py` from the top-level hil directory. Parallel testing can be used on multi-core systems by running `py.test tests/unit tests/stress.py -n auto`
  - [ ] Add unit tests in the corresponding file and create one if none are present.
  - [ ] If practical, bug fixes should have an reproducing test to ensure that the bug does not come back.
  - [ ] Run deployment tests if code could affect switches
- [ ] Reviewed and approved by at least two other main contributors or one for simple documentation change.
