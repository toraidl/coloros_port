# Contributing

Thanks for helping improve the ColorOS porting tools. Please check the target branch and device before opening an issue or pull request; behavior can differ across branches and ROM builds.

## Report a problem

Use the [bug report form](https://github.com/toraidl/coloros_port/issues/new?template=bug_report.yml) and include, where applicable:

- Device model and codename
- Branch, base ROM build, and port ROM build
- Host operating system and architecture
- The exact step where the problem occurs, with steps to reproduce
- Relevant sanitized output and what you expected to happen

Do not attach complete ROM packages, proprietary files, private keys, device serial numbers, access tokens, or personal data. Redact those values from logs before posting.

## Open a pull request

- Target the branch that matches the affected Android / ROM generation. Check the repository branches if you are unsure.
- Keep the change focused and explain the user-facing problem it solves.
- Include the commands or checks you ran and their results. If you could not test on a matching device or ROM build, say so and list what remains unverified.
- For device-specific changes, include the device codename and exact base and port builds used for verification.
- Do not add firmware packages, proprietary blobs, credentials, signing keys, or generated build outputs unless the repository maintainers have confirmed that they belong in the change and may be redistributed.

## Review expectations

Changes to porting and flashing scripts can affect device data and bootability. Pull requests should make their target branch, host environment, and device-side verification status clear so maintainers can review the scope and risks.
