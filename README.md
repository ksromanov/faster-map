This fork of `faster-map` is used for benchmarking TRMC project.

To measure the speed of TRMC map:

1. Install new switch with TRMC compiler:
    * `git clone` to `~/ocaml`, checkout proper branch
    * remove `"ocaml" {= "4.10.1" & post}` dependency from `ocaml-variants.opam` in the repo
    * Add switch: `opam switch create --empty frederic_trmc_4_10_correct; cd ~/ocaml; opam pin .`

2. Do not set `OCAMLPARAM="force_trmc=1,_"`!

3. Run `make`, the resulting picture will be in `./_report/map.svg`
