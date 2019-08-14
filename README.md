# using-yaml-repro

Repro of issue:

    chris@precision:~/Work/simspace/using-yaml-repro$ git log --oneline -n 1
    275bb04 (HEAD -> master) Repro of #4096
    chris@precision:~/Work/simspace/using-yaml-repro$ stack build
    /tmp/hpack-pkg-dir7171/package.yaml: Yaml file not found: /tmp/package-common.yaml
    chris@precision:~/Work/simspace/using-yaml-repro$

Fix of issue:

    chris@precision:~/Work/simspace/using-yaml-repro$ git log --oneline -n 1
    b6209c5 (HEAD -> master) Fix for #4096
    chris@precision:~/Work/simspace/using-yaml-repro$ stack build
    Building all executables for `using-yaml-repro' once. After a successful build of all of them, only specified executables will be rebuilt.
    using-yaml-repro> configure (lib + exe)
    Configuring using-yaml-repro-0.1.0.0...
    using-yaml-repro> build (lib + exe)
    Preprocessing library for using-yaml-repro-0.1.0.0..
    Building library for using-yaml-repro-0.1.0.0..
    [1 of 2] Compiling Lib
    [2 of 2] Compiling Paths_using_yaml_repro
    Preprocessing executable 'using-yaml-repro-exe' for using-yaml-repro-0.1.0.0..
    Building executable 'using-yaml-repro-exe' for using-yaml-repro-0.1.0.0..
    [1 of 2] Compiling Main
    [2 of 2] Compiling Paths_using_yaml_repro
    Linking .stack-work/dist/x86_64-linux/Cabal-2.4.0.1/build/using-yaml-repro-exe/using-yaml-repro-exe ...
    using-yaml-repro> copy/register
    Installing library in /home/chris/Work/simspace/using-yaml-repro/.stack-work/install/x86_64-linux/36e4db1b7f301090305a0703c612d386ebee75f61b14dc525f0ee770b1d908a0/8.6.5/lib/x86_64-linux-ghc-8.6.5/using-yaml-repro-0.1.0.0-Jj5rHuI4X6qbKOKNPw504
    Installing executable using-yaml-repro-exe in /home/chris/Work/simspace/using-yaml-repro/.stack-work/install/x86_64-linux/36e4db1b7f301090305a0703c612d386ebee75f61b14dc525f0ee770b1d908a0/8.6.5/bin
    Registering library for using-yaml-repro-0.1.0.0..
    chris@precision:~/Work/simspace/using-yaml-repro$
