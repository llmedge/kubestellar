# Kubestellar singleton status return

This test is an executable variant of the singleton status scenario in [the examples doc](../../../docs/content/v0.20/examples.md). This test has the same prerequisites as the cited one. This test can test either (a) the  local copy of the repo or (b) the release identified in the kubestellar PostCreateHook (which will be the last release created, regardless of quality, except for that brief time when it identifies the release about to be made). Testing the local copy is the default behavior; to test the release identified in the PostCreateHook, pass `--released` on the command line of `run-test.sh`.

## Running the test using a script

Starting from a local directory containing the git repo, do the following.

```
cd test/e2e/singleton-status
./run-test.sh
```
