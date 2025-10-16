This one is for glibc-2.17, which lacks many conda packages and thus relay on host for libs.

1. Install pixi with `curl -fsSL https://pixi.sh/install.sh | sh`.
2. `cd /lustre/software/pixi/gpu4pyscf`
3. `pixi install`. The only source file is `/lustre/software/pixi/gpu4pyscf/pixi.toml`.
4. `pixi shell`
5. `which python3` to get its full path.
6. Add that path, "/lustre/software/pixi/gpu4pyscf/.pixi/envs/default/bin" to $PATH.
 
