Goals:
 - Figure out where we are at.
 - what/why multi stage container builds
 - adding that to a github action
 - Chainguard images / what why how when
 - Pipeline security with Sigstore

Takeaways:
 - how important easy updates are.
 - need a clean opensource way (via gitops?) to (docker watchtower?)
 - distroless - removed a lot of the classic userspace software (no package manager ect)

Where we are:
Prod: 2 critical, 20 high, 32 medium, 7 low, 58 negligible (36 unknown)
rebuild: 0 critical, 0 high, 26 medium, 20 low, 3 negligible
171mb

Where did we get:
31.4MB (still need to add openssl) less then 40.
0 critical, 0 high, 0 medium, 0 low, 0 negligible

TODO: 15 minute video recap - go over whatever the issue is currently with our OIDC signing in github actions.