# GPG Signing

Re-enable and enhance the GPG signing step to sign the Helm package before pushing it to the `Reaper` repository.

```
# - name: sign-off
#   inputs: {}
#   outputs: {}
#   metadata: {}
#   container:
#     name: ''
#     image: alpine
#     command:
#       - sh
#       - '-c'
#     args:
#       - |
#         gpg --import /path/to/private.key && \
#         gpg --batch --yes --passphrase-fd 0 --pinentry-mode loopback --sign --output /workspace/input-repo/signed-package.tar.gz /workspace/input-repo/package.tar.gz || { echo "GPG sign-off failed"; exit 1; }
#     resources: {}
#     volumeMounts:
#       - name: workspace
#         mountPath: /workspace
#       - name: gpg-key
#         mountPath: /path/to

```
