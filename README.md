#### A minimalist .env support for Neovim 

# Prerequisites

Neovim 0.7.0+

# Installing

Using `packer`

```lua
use { "amihere/dotenv.nvim" }
```

# Basic Usage

```lua
require('dotenv').setup()
```

# Configuration

Additional settings are:

```lua
require('dotenv').setup({
  enable_on_load = true, -- will load your .env file upon loading a buffer
  verbose = false, -- show error notification if .env file is not found and if .env is loaded
})
```

# Usage

## Loading .env

If you prefer to not load the .env file upon opening a file, you can use the user command:

```
:Dotenv
```

Optionally use a file as param, if the file is not in the current directory

```
:Dotenv PATH
```

## Inspecting an env (must load env first)

```
:DotenvGet ENV
```
