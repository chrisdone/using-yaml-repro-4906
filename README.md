# using-yaml-repro

Repro of issue:

    chris@precision:~/Work/simspace/using-yaml-repro$ git log --oneline -n 1
    275bb04 (HEAD -> master) Repro of #4096
    chris@precision:~/Work/simspace/using-yaml-repro$ stack build
    /tmp/hpack-pkg-dir7171/package.yaml: Yaml file not found: /tmp/package-common.yaml
    chris@precision:~/Work/simspace/using-yaml-repro$
