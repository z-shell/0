<h2 align="center">
  <a href="https://github.com/z-shell/zi">
    <img src="https://github.com/z-shell/zi/raw/main/docs/images/logo.svg" alt="Logo" width="80" height="80" />
  </a>
❮ ZI ❯ Plugin - Null
</h2>

An empty repository to aid ZI atclone'' hook.

Use case example: 

```
# The invocation uses https://github.com/z-shell/null repo as a placeholder
# for the atclone'' and atpull'' hooks

zi ice as"program" pick"$ZPFX/sdkman/bin/sdk" id-as'sdkman' run-atpull \
  atclone"wget https://get.sdkman.io -O scr.sh; SDKMAN_DIR=$ZPFX/sdkman bash scr.sh" \
  atpull"SDKMAN_DIR=$ZPFX/sdkman sdk selfupdate" \
  atinit"export SDKMAN_DIR=$ZPFX/sdkman; source $ZPFX/sdkman/bin/sdkman-init.sh"
zi light z-shell/null
```
