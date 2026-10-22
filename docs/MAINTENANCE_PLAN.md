# Maintenance Plan | 维护计划

This is a proposed roadmap, not a promise of release dates. Compatibility claims should be updated only after a matching device and ROM combination has been checked.

这是一个维护路线提案，不代表承诺发布日期。只有在对应设备和 ROM 组合经过验证后，才应更新兼容性声明。

## Baseline | 当前情况

- The repository targets ColorOS / OxygenOS porting across Android 14–17 branches. Device and ROM compatibility varies by branch.
- The default branch has Android 17 support commits dated 2026-08-13 and 2026-08-14.
- The public GitHub page showed 96 stars and 53 forks on 2026-10-22. These are point-in-time interest signals, not download or active-user counts.
- A GitHub Release named `assets` was published on 2026-03-03. The repository does not publish a verified monthly download figure in its README.

## Stage 1 — Make the project easier to evaluate and contribute to

Completed in this proposal:

- Refresh the Chinese and English READMEs, fix the clone URL, explain branch-specific support, and label old test notes as historical.
- Add a contribution guide that asks for the exact device, branch, ROM builds, host, and verification status.
- Add a bug report form that collects reproducible details and warns reporters not to upload ROM packages, secrets, or personal data.

## Stage 2 — Publish a verified compatibility record

- Track each verified combination with device model and codename, target branch, base and port ROM builds, test date, boot status, key functions checked, and known limitations.
- Keep untested or user-reported combinations clearly marked; do not generalize one device's result to every device in a series.
- Update the README or release notes when a new combination is verified.

## Stage 3 — Improve release traceability

- Use a release title that identifies the project version or source commit instead of a generic name.
- Include the target branches and devices, exact ROM builds when relevant, changes, known limitations, and verification status in release notes.
- Publish checksums for downloadable assets. Keep proprietary files out of Git and publish binary assets only when redistribution is permitted.

## Stage 4 — Add safe, repeatable checks

- Identify deterministic checks for the project's shell scripts and Python utilities, then run them on proposed changes.
- Add lightweight CI for checks that do not require proprietary ROM images or connected phones.
- Keep device flashing and other destructive hardware actions out of automated CI.

## Ongoing maintainer workflow

- Triage incoming reports by requesting missing device, branch, ROM, and reproduction details.
- Review changes against the target branch and record what was actually tested, including limitations.
- Refresh compatibility and release information when there is new verified evidence.

## Reporting project evidence

When describing this project to a sponsor or another maintainer program, use dated public evidence. State the device-porting niche and the work needed to maintain compatibility across Android generations. Do not claim monthly downloads, broad adoption, or current feature support without a source. Choose a primary or core maintainer role based on the applicant's real ongoing responsibilities and repository access.
