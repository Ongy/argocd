# ongy argocd repo

This repository contains the argocd applications I use for my home cluster.

This is provided as-is with no intention to be useful to others, but is mostly a reference for my blog posts and my backup.

If you can make use of something with minor changes, I'm likely to accept a PR though.

## URLs

Note that the URLs point at an internal server. This is the actual SoT for this data.
The internal server is useful because it allows two things:
* Work fully offline
* trigger webhook handlers within my network

The `argo-workflows-git-sync` dir provides one such webhook handler. It copies out repositories I SoT internally to github.