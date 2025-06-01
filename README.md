```bash
# See https://docs.gradle.org/current/userguide/part1_gradle_init.html
gradle init
```

```lua
-- Using github:mfussenegger/nvim-jdtls
-- See full config on https://github.com/hooreique/hoo-nvim-conf/blob/main/lua/plugins/jdtls.lua
vim.api.nvim_create_autocmd("FileType", {
  pattern = "java",
  callback = function()
    require('jdtls').start_or_attach {
      cmd = {
        'jdtls',
        '-data',
        datadir, -- 💀
      },
    }
  end,
})
```
