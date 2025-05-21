# Contributing

This repository relates to activities in the Internet Engineering Task Force
([IETF](https://www.ietf.org/)). All material in this repository is considered
Contributions to the IETF Standards Process, as defined in the intellectual
property policies of IETF currently designated as
[BCP 78](https://www.rfc-editor.org/info/bcp78),
[BCP 79](https://www.rfc-editor.org/info/bcp79) and the
[IETF Trust Legal Provisions (TLP) Relating to IETF Documents](http://trustee.ietf.org/trust-legal-provisions.html).

Any edit, commit, pull request, issue, comment or other change made to this
repository constitutes Contributions to the IETF Standards Process
(https://www.ietf.org/).

You agree to comply with all applicable IETF policies and procedures, including,
BCP 78, 79, the TLP, and the TLP rules regarding code components (e.g. being
subject to a Simplified BSD License) in Contributions.


## Working Group Information

Discussion of this work occurs on the [MODeration PrOceDures
Working Group mailing list](mailto:mod-discuss@ietf.org)
([archive](https://mailarchive.ietf.org/arch/browse/mod-discuss/),
[subscribe](https://mailman3.ietf.org/mailman3/lists/mod-discuss.ietf.org/)).
In addition to contributions in GitHub, you are encouraged to participate in
discussions there.

**Note**: Some working groups adopt a policy whereby substantive discussion of
technical issues needs to occur on the mailing list.

You might also like to familiarize yourself with other
[Working Group documents](https://datatracker.ietf.org/wg/modpod/documents/).

## Markdown Lint Instructions

This repository runs `markdown-lint` as a GitHub Workflow when a PR is
submitted. It can be run locally using Docker with an identical configuration
to the GitHub Workflow.

```bash
docker run --rm \
-v "$(pwd)/draft-ietf-modpod-group-processes.md:\
/draft-ietf-modpod-group-processes.md:ro" \
-v "$(pwd)/.github/workflows/markdownlint.json:\
/markdownlint.json:ro" \
avtodev/markdown-lint:v1 \
--config ./markdownlint.json \
/draft-ietf-modpod-group-processes.md
```
