## Vscode Settings and extensions

Setting them up, from terminal:

```sh
foo@bar:~$ git clone https://github.com/Lucas-Fonte/vscode.git
foo@bar:~$ cd vscode
foo@bar:~$ bash vscode_extensions.sh
foo@bar:~$ code .
```

Then with vscode opened, <kbd>command/ctrl</kbd> + <kbd>shift</kbd> + <kbd>P</kbd> ">Open Settings (JSON)", paste the file **settings.json**.

### To extract the extensions

```sh
foo@bar:~$ code --list-extensions | sed -e 's/^/code --install-extension /' > my_vscode_extensions.sh
```

