export CONDA_PREFIX=/lustre/software/pixi/gpu4pyscf/.pixi/envs/default
export PIXI_PROMPT='(gpu4pyscf) '
export PIXI_PROJECT_NAME=gpu4pyscf
export PIXI_ENVIRONMENT_NAME=default
export CONDA_SHLVL=1
export PATH=/lustre/software/pixi/gpu4pyscf/.pixi/envs/default/bin:/usr/java/jre1.8.0_151/bin:/usr/java/jre1.8.0_151/bin:/lustre/software/tsce4/torque6/bin:/lustre/software/tsce4/torque6/sbin:/usr/local/bin:/usr/lib64/qt-3.3/bin:/lustre/home/xshu/perl5/bin:/usr/bin:/bin:/usr/sbin:/sbin:/usr/local/sbin:.:/lustre/software/bin/
export PIXI_ENVIRONMENT_PLATFORMS=linux-64
export PIXI_EXE=/lustre/software/pixi/.bin/pixi
export PIXI_PROJECT_MANIFEST=/lustre/software/pixi/gpu4pyscf/pixi.toml
export PIXI_PROJECT_VERSION=0.1.0
export CONDA_DEFAULT_ENV=gpu4pyscf
export PIXI_IN_SHELL=1
export PIXI_PROJECT_ROOT=/lustre/software/pixi/gpu4pyscf
echo PIXI_SHELL_ACTIVATION_DONE
export PS1="(gpu4pyscf) ${PS1:-}"
# shellcheck shell=bash
pixi() {
    local first_arg="${1-}"

    "${PIXI_EXE-}" "$@" || return $?

    case "${first_arg-}" in
    add | a | remove | rm | install | i)
        eval "$("$PIXI_EXE" shell-hook --change-ps1 false)"
        hash -r
        ;;
    esac || :

    return 0
}
