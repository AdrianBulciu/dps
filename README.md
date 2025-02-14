
# dps (docker ps)

A faster way of using 'docker ps' combined with a shell 'docker exec'

## Installation

Download & Unzip the project:

```
curl -L -O https://github.com/AdrianBulciu/dps/archive/main.zip

unzip main.zip
```

Run the install script:

```
cd dps-main

sudo ./install
```

That's it, now you should be able to invoke the script by writing 'dps' in the terminal.
    
## Optional settings

There is a config file options.config where you can change the following:

```
RENDER_MENU_AFTER_CONTAINER_EXIT=FALSE
SHELLS=('bash' 'sh')
```

You can also configure what info to show about every container in the template.tmpl file.

```
table {{.ID}}\t{{.Image}}\t{{.Names}}\t{{.State}}\t{{.Status}}\t{{.RunningFor}}
```

#### Important: ID or Name must be the first element of the template!

After making changes to settings or the template you must run the install script again.

## Demo

https://github.com/user-attachments/assets/0bdc9601-0f5d-4397-bd76-878b27c5d890

## License

[GPL license](LICENSE.md)
